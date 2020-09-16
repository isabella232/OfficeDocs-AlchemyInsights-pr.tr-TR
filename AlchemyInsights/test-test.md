---
title: SharePoint Online terim deposunda terimler eksik
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750471"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="5df86-102">Intune ile BitLocker şifrelemesini etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="5df86-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="5df86-103">Intune, Intune kullanarak cihazları korumada açıklandığı gibi Windows cihazları için Boitkilitsiz şifreleme ayarlarını yapılandırmak için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="5df86-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="5df86-104">Windows 10 çalıştıran yeni aygıtların, MDM ilkesinin uygulaması olmadan tetiklenen otomatik BitLocker şifrelemesini desteklemediğini bilmelisiniz.</span><span class="sxs-lookup"><span data-stu-id="5df86-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="5df86-105">Bu, varsayılan ayarlar yapılandırılmadığında ilkenin uygulamasını etkileyebilir.</span><span class="sxs-lookup"><span data-stu-id="5df86-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="5df86-106">Daha ayrıntılı bilgi için SSS bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="5df86-106">See FAQ for more detail.</span></span>


<span data-ttu-id="5df86-107">SSS   : Windows 'un hangi sürümleri Endpoint Protection ilkesini kullanarak cihaz şifrelemeyi destekliyor mu?</span><span class="sxs-lookup"><span data-stu-id="5df86-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="5df86-108"> A: Intune Endpoint Protection Ilkesindeki ayarlar BitLocker CSP kullanılarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="5df86-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="5df86-109">Windows 'un tüm sürümleri ve derlemeleri BitLocker CSP 'yi desteklemez. 
     </span><span class="sxs-lookup"><span data-stu-id="5df86-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="5df86-110">Şu anda Windows sürümlerinde: Kurumsal; Eğitim, mobil, mobil kurumsal ve profesyonel (derleme 1809 sürümleri) desteklenir.</span><span class="sxs-lookup"><span data-stu-id="5df86-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="5df86-111">S: bir cihaz zaten BitLocker ile şifrelenmiş şifreleme yönteminin varsayılan ayarları ve şifreleme gücü (XTS-AES-128) kullanılarak şifrelenmişse, farklı ayarlarla ilke uygulanarak yeni ayarlarla sürücünün yeniden şifrelenmesi otomatik olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="5df86-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="5df86-112">Y: Hayır.</span><span class="sxs-lookup"><span data-stu-id="5df86-112">A: No.</span></span> <span data-ttu-id="5df86-113">Yeni şifre ayarlarını uygulamak için önce sürücünün şifresinin çözülmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="5df86-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="5df86-114">Autopilot ile kaydolan cihazların, Intune ilkesi değerlendirilinceye kadar otomatik şifreleme tetiklenemez ve bu da işletim sisteminin Varsayılanları yerine ilke tabanlı ayarların kullanılmasına izin verir</span><span class="sxs-lookup"><span data-stu-id="5df86-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="5df86-115">S Intune ilkesi uygulaması nedeniyle bir cihaz şifrelenmişse, bu ilke kaldırıldığında şifresi çözülür mi?</span><span class="sxs-lookup"><span data-stu-id="5df86-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="5df86-116">A: şifrelemeyle ilgili ilkenin kaldırılması, yapılandırılmış sürücülerin şifresinin çözülmesini sağlamaz.</span><span class="sxs-lookup"><span data-stu-id="5df86-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="5df86-117">S: Intune uyumluluk ilkesinde neden cihazımın "BitLocker etkin" olduğunu gösteriyor, ancak şu mu?</span><span class="sxs-lookup"><span data-stu-id="5df86-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="5df86-118">A: Intune uyumluluk ilkesindeki "BitLocker etkin" ayarı, Windows cihaz durumu kanıtlama (DHA) istemcisinin kullanır.</span><span class="sxs-lookup"><span data-stu-id="5df86-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="5df86-119">Bu istemci yalnızca önyükleme sırasında cihaz durumunu ölçtüğünden.</span><span class="sxs-lookup"><span data-stu-id="5df86-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="5df86-120">Bu nedenle, BitLocker şifrelemesi tamamlandığından bir cihaz yeniden başlatılıncaya kadar, DHA istemci hizmeti BitLocker 'ı etkin olduğu gibi bildirmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="5df86-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>