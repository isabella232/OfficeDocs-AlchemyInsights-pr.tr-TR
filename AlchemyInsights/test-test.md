---
title: SharePoint Online Term Store'dan eksik terimler
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053533"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="87d7c-102">Intune ile Bitlocker Şifrelemesini Etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="87d7c-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="87d7c-103">Intune Endpoint Protection Policy, Windows aygıtları için Boitlocker şifreleme ayarlarını açıklandığı gibi yapılandırmak için kullanılabilir: Windows10 (ve sonraki) ayarlarını Intune kullanan aygıtları korumak için</span><span class="sxs-lookup"><span data-stu-id="87d7c-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="87d7c-104">Windows 10 çalıştıran birçok yeni aygıtın MDM ilkesi uygulaması olmadan tetiklenen otomatik bitlocker şifrelemesini desteklediğini unutmayın.</span><span class="sxs-lookup"><span data-stu-id="87d7c-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="87d7c-105">Varsayılan olmayan ayarlar yapılandırılırsa, bu ilkenin uygulanmasını etkileyebilir.</span><span class="sxs-lookup"><span data-stu-id="87d7c-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="87d7c-106">Daha fazla ayrıntı için SSS bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="87d7c-106">See FAQ for more detail.</span></span>


<span data-ttu-id="87d7c-107"> SSS S: Son Nokta Koruma İlkesi'ni kullanarak Windows'un aygıt şifrelemesini destekleyen sürümleri?</span><span class="sxs-lookup"><span data-stu-id="87d7c-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="87d7c-108"> C: Intune Endpoint Protection Policy'deki ayarlar Bitlocker CSP kullanılarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="87d7c-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="87d7c-109">Tüm sürümleri veya Windows yapıları Bitlocker CSP'yi desteklemez. 
     </span><span class="sxs-lookup"><span data-stu-id="87d7c-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="87d7c-110">Şu anda Windows Editions: Enterprise; Eğitim, Mobil, Mobil Kurumsal ve Profesyonel (1809'dan itibaren) desteklenir.</span><span class="sxs-lookup"><span data-stu-id="87d7c-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="87d7c-111">S: Bir aygıt şifreleme yöntemi ve şifreleme gücü (XTS-AES-128) için işletim sistemi varsayılan ayarlarını kullanarak Bitlocker ile zaten şifrelenmişse, farklı ayarlara sahip bir ilke uygulayacak sayılsa, yeni ayarlarla sürücünün yeniden şifrelemesini otomatik olarak tetikler mi?</span><span class="sxs-lookup"><span data-stu-id="87d7c-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="87d7c-112">C: Hayır.</span><span class="sxs-lookup"><span data-stu-id="87d7c-112">A: No.</span></span> <span data-ttu-id="87d7c-113">Yeni şifreleme ayarlarını uygulamak için öncelikle sürücünün şifresinin çözülmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="87d7c-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="87d7c-114">Not Otomatik Pilot'a kayıtlı olan aygıtlar için, INtune ilkesi değerlendirilene kadar OOBE sırasında oluşacak otomatik şifreleme tetiklenmez ve bu da işletim sistemi varsayılanları yerine ilke tabanlı ayarların kullanılmasına izin verir</span><span class="sxs-lookup"><span data-stu-id="87d7c-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="87d7c-115">S Bir aygıt Intune ilkesinin uygulanması sonucunda şifrelenirse, bu ilke kaldırıldığında şifresi çözülür mü?</span><span class="sxs-lookup"><span data-stu-id="87d7c-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="87d7c-116">C: Şifreleme ile ilgili ilke kaldırılması, yapılandırılan sürücülerin şifresinin çözülmesiyle sonuçlanmaz.</span><span class="sxs-lookup"><span data-stu-id="87d7c-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="87d7c-117">S: Intune Uyumluluk ilkesi, aygıtımda "Bitlocker Etkin" olmadığını, ancak etkin olduğunu neden gösteriyor?</span><span class="sxs-lookup"><span data-stu-id="87d7c-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="87d7c-118">C: Intune uyumluluk ilkesinde "Bitlocker etkin" ayarı Windows Aygıt Durumu Attestation (DHA) istemcisini kullanır.</span><span class="sxs-lookup"><span data-stu-id="87d7c-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="87d7c-119">Bu istemci yalnızca önyükleme zamanında aygıt durumunu ölçer.</span><span class="sxs-lookup"><span data-stu-id="87d7c-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="87d7c-120">Bu nedenle, bitlocker şifrelemesi tamamlandığından beri bir aygıt yeniden başlatılmazsa, DHA istemci hizmeti bitlocker'ı etkin olarak bildirmez.</span><span class="sxs-lookup"><span data-stu-id="87d7c-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>