---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731259"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="d2fac-102">Intune ile BitLocker şifrelemesini etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="d2fac-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="d2fac-103">Windows cihazlarında BitLocker şifreleme ayarlarını yapılandırmak için Intune Endpoint Protection Ilkesi kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="d2fac-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="d2fac-104">Daha fazla bilgi için, [Intune kullanarak cihazları korumada Windows 10 (ve sonraki sürümler) ayarlarına](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)bakın.</span><span class="sxs-lookup"><span data-stu-id="d2fac-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="d2fac-105">Windows 10 çalıştıran yeni aygıtların, MDM ilkesi uygulaması olmadan tetiklenen otomatik BitLocker şifrelemesini desteklemediğini bilmelisiniz.</span><span class="sxs-lookup"><span data-stu-id="d2fac-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="d2fac-106">Bu, varsayılan olmayan ayarlar yapılandırılırsa ilkenin uygulamasını etkileyebilir.</span><span class="sxs-lookup"><span data-stu-id="d2fac-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="d2fac-107">Daha ayrıntılı bilgi için aşağıdaki SSS bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="d2fac-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="d2fac-108">BitLocker sorunlarını giderme hakkında bilgi için [Microsoft Intune 'Da BitLocker Ilkelerinde sorun giderme](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="d2fac-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="d2fac-109">**SSS**</span><span class="sxs-lookup"><span data-stu-id="d2fac-109">**FAQ**</span></span>

 <span data-ttu-id="d2fac-110">S: Endpoint Protection Ilkesini kullanarak Windows 'un hangi sürümleri cihaz şifrelemesini destekliyor?</span><span class="sxs-lookup"><span data-stu-id="d2fac-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="d2fac-111">A: Intune Endpoint Protection Ilkesindeki ayarlar [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)kullanılarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="d2fac-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="d2fac-112">Tüm Windows sürümleri veya derlemeleri BitLocker CSP 'yi desteklemez.</span><span class="sxs-lookup"><span data-stu-id="d2fac-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="d2fac-113">Şu anda, aşağıdaki Windows sürümleri desteklenir: Kurumsal, eğitim, mobil, mobil kurumsal ve profesyonel (derleme 1809 ve üstü).</span><span class="sxs-lookup"><span data-stu-id="d2fac-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="d2fac-114">S: cihaz zaten şifreleme yöntemi ve şifreleme gücü (XTS-AES-128) için işletim sistemi varsayılan ayarları kullanılarak bir cihaz şifrelenmişse, farklı ayarlarla bir ilke uygulama yeni ayarlarla otomatik olarak yeniden şifrelemeyi tetikleyecektir.</span><span class="sxs-lookup"><span data-stu-id="d2fac-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="d2fac-115">Y: Hayır.</span><span class="sxs-lookup"><span data-stu-id="d2fac-115">A: No.</span></span> <span data-ttu-id="d2fac-116">Yeni şifre ayarlarını uygulamak için önce sürücünün şifresinin çözülmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="d2fac-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="d2fac-117">**Not:** Autopilot 'e Kaydolmakta olan cihazlar için, Intune ilkesi değerlendirilinceye kadar OOBE sırasında oluşacak Otomatik şifreleme tetiklenemez ve bu da işletim sistemi varsayılanları yerine ilke tabanlı ayarların kullanılmasına olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="d2fac-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="d2fac-118">S: Intune ilkesi uygulamasının bir sonucu olarak bir cihaz şifrelenmişse, bu ilke kaldırıldığında şifresi çözülür mi?</span><span class="sxs-lookup"><span data-stu-id="d2fac-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="d2fac-119">A: şifrelemeyle ilgili ilkenin kaldırılması, yapılandırılmış sürücülerin şifresinin çözülmesini sağlamaz.</span><span class="sxs-lookup"><span data-stu-id="d2fac-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="d2fac-120">S: Intune uyumluluk Ilkesinde neden aygıtımın BitLocker 'ın etkin olmadığını gösterir, ancak olsa da?</span><span class="sxs-lookup"><span data-stu-id="d2fac-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="d2fac-121">A: Intune uyumluluk Ilkesindeki "BitLocker etkin" ayarı Windows cihaz durumu kanıtlama (DHA) istemcisini kullanır.</span><span class="sxs-lookup"><span data-stu-id="d2fac-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="d2fac-122">Bu istemci yalnızca önyükleme sırasında cihaz durumunu ölçtüğünden.</span><span class="sxs-lookup"><span data-stu-id="d2fac-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="d2fac-123">Bu nedenle, BitLocker şifrelemesi tamamlandığından bir cihaz yeniden başlatılıncaya kadar, DHA istemci hizmeti BitLocker 'ı etkin olduğu gibi bildirmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="d2fac-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 