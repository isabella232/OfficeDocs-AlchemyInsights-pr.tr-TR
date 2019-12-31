---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908729"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="9031b-102">Intune ile Bitlocker şifrelemesini etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="9031b-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="9031b-103">Intune Endpoint Protection Policy, Windows aygıtları için Bitlocker şifreleme ayarlarını yapılandırmak için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="9031b-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="9031b-104">Daha fazla bilgi için, [Intune kullanan aygıtları korumak için Windows 10 (ve sonraki) ayarlarına](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)bakın.</span><span class="sxs-lookup"><span data-stu-id="9031b-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="9031b-105">Windows 10 çalıştıran birçok yeni aygıtın MDM ilkesi uygulanmadan tetiklenen otomatik Bitlocker şifrelemesini desteklediğini unutmayın.</span><span class="sxs-lookup"><span data-stu-id="9031b-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="9031b-106">Varsayılan olmayan ayarlar yapılandırılırsa, bu ilkenin uygulanmasını etkileyebilir.</span><span class="sxs-lookup"><span data-stu-id="9031b-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="9031b-107">Daha fazla ayrıntı için aşağıdaki SSS bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="9031b-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="9031b-108">Bitlocker sorun giderme sorunları hakkında daha fazla bilgi için [Microsoft Intune'daki Sorun Giderme BitLocker ilkelerine](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)bakın.</span><span class="sxs-lookup"><span data-stu-id="9031b-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="9031b-109">**SSS**</span><span class="sxs-lookup"><span data-stu-id="9031b-109">**FAQ**</span></span>

 <span data-ttu-id="9031b-110">S: Endpoint Protection İlkesi'ni kullanarak Windows destek aygıt şifrelemesinin hangi sürümleri?</span><span class="sxs-lookup"><span data-stu-id="9031b-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="9031b-111">C: Intune Endpoint Protection Policy'deki ayarlar [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)kullanılarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="9031b-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="9031b-112">Windows'un tüm sürümleri veya yapıları Bitlocker CSP'yi desteklemez.</span><span class="sxs-lookup"><span data-stu-id="9031b-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="9031b-113">Şu anda aşağıdaki Windows sürümleri desteklenir: Enterprise, Education, Mobile, Mobile Enterprise ve Professional (1809 ve sonrası oluşturun).</span><span class="sxs-lookup"><span data-stu-id="9031b-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="9031b-114">S: Bir aygıt şifreleme yöntemi ve şifreleme gücü (XTS-AES-128) için işletim sistemi varsayılan ayarlarını kullanarak Bitlocker ile zaten şifrelenmişse, farklı ayarlara sahip bir ilke uygulamak sürücünün yeni ayarlarla otomatik olarak yeniden şifrelemesini tetikler mi?</span><span class="sxs-lookup"><span data-stu-id="9031b-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="9031b-115">C: Hayır.</span><span class="sxs-lookup"><span data-stu-id="9031b-115">A: No.</span></span> <span data-ttu-id="9031b-116">Yeni şifreleme ayarlarını uygulamak için önce sürücünün şifresinin çözülmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="9031b-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="9031b-117">**Not:** Otomatik Pilot'a kaydolan aygıtlar için, INtune ilkesi değerlendirilene kadar OOBE sırasında oluşacak otomatik şifreleme tetiklenmez ve bu da işletim sistemi varsayılanları yerine ilke tabanlı ayarların kullanılmasına olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="9031b-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="9031b-118">S: Bir aygıt Intune ilkesinin uygulanması sonucunda şifrelenirse, bu ilke kaldırıldığında şifresi çözülür mü?</span><span class="sxs-lookup"><span data-stu-id="9031b-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="9031b-119">C: Şifrelemeyle ilgili ilkekaldırılması, yapılandırılan sürücülerin şifresinin çözülmesiyle sonuçlanmaz.</span><span class="sxs-lookup"><span data-stu-id="9031b-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="9031b-120">S: Intune Uyumluluk İlkesi, aygıtımda bitlocker etkin olmadığını neden gösteriyor?</span><span class="sxs-lookup"><span data-stu-id="9031b-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="9031b-121">C: Intune Uyumluluk İlkesi'ndeki "Bitlocker etkin" ayarı, Windows Aygıt Durumu Attestation (DHA) istemcisini kullanır.</span><span class="sxs-lookup"><span data-stu-id="9031b-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="9031b-122">Bu istemci yalnızca önyükleme zamanında aygıt durumunu ölçer.</span><span class="sxs-lookup"><span data-stu-id="9031b-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="9031b-123">Bu nedenle, Bitlocker şifrelemesi tamamlandığından beri bir aygıt yeniden başlatılmazsa, DHA istemci hizmeti Bitlocker'ı etkin olarak bildirmez.</span><span class="sxs-lookup"><span data-stu-id="9031b-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 