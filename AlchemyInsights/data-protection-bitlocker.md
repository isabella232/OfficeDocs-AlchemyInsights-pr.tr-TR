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
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768837"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="3d710-102">Intune ile BitLocker şifrelemesini etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="3d710-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="3d710-103">Windows cihazlarında BitLocker şifreleme ayarlarını yapılandırmak için Intune Endpoint Protection Ilkesi kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="3d710-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="3d710-104">Daha fazla bilgi için, [Intune kullanarak cihazları korumada Windows 10 (ve sonraki sürümler) ayarlarına](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)bakın.</span><span class="sxs-lookup"><span data-stu-id="3d710-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="3d710-105">Windows 10 çalıştıran yeni aygıtların, MDM ilkesi uygulaması olmadan tetiklenen otomatik BitLocker şifrelemesini desteklemediğini bilmelisiniz.</span><span class="sxs-lookup"><span data-stu-id="3d710-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="3d710-106">Bu, varsayılan olmayan ayarlar yapılandırılırsa ilkenin uygulamasını etkileyebilir.</span><span class="sxs-lookup"><span data-stu-id="3d710-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="3d710-107">Daha ayrıntılı bilgi için aşağıdaki SSS bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="3d710-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="3d710-108">BitLocker sorunlarını giderme hakkında bilgi için [Microsoft Intune 'Da BitLocker Ilkelerinde sorun giderme](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="3d710-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="3d710-109">**SSS**</span><span class="sxs-lookup"><span data-stu-id="3d710-109">**FAQ**</span></span>

<span data-ttu-id="3d710-110">S: Endpoint Protection Ilkesini kullanarak Windows 'un hangi sürümleri cihaz şifrelemesini destekliyor?</span><span class="sxs-lookup"><span data-stu-id="3d710-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="3d710-111">A: Intune Endpoint Protection Ilkesindeki ayarlar [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)kullanılarak uygulanır.</span><span class="sxs-lookup"><span data-stu-id="3d710-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="3d710-112">Tüm Windows sürümleri veya derlemeleri BitLocker CSP 'yi desteklemez.</span><span class="sxs-lookup"><span data-stu-id="3d710-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="3d710-113">S: Son Kullanıcı etkileşimi gerekmeden cihazlarda BitLocker nasıl etkinleştirilebilir?</span><span class="sxs-lookup"><span data-stu-id="3d710-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="3d710-114">A: gerekli önkoşulları karşıladığı için, Intune aracılığıyla BitLocker "sessiz şifrelemeyi" etkinleştirmeniz olasıdır.</span><span class="sxs-lookup"><span data-stu-id="3d710-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="3d710-115">Aşağıdaki belgede sessiz şifrelemeyi etkinleştirmek için cihaz gereksinimleri ve örnek ilke ayarlarının ayrıntılarına bakın: [BitLocker şifrelemesini sessizce etkinleştirin](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="3d710-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="3d710-116">S: cihaz zaten şifreleme yöntemi ve şifreleme gücü (XTS-AES-128) için işletim sistemi varsayılan ayarları kullanılarak bir cihaz şifrelenmişse, farklı ayarlarla bir ilke uygulama yeni ayarlarla otomatik olarak yeniden şifrelemeyi tetikleyecektir.</span><span class="sxs-lookup"><span data-stu-id="3d710-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="3d710-117">Y: Hayır.</span><span class="sxs-lookup"><span data-stu-id="3d710-117">A: No.</span></span> <span data-ttu-id="3d710-118">Yeni şifre ayarlarını uygulamak için önce sürücünün şifresinin çözülmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="3d710-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="3d710-119">**Not:** Autopilot 'e Kaydolmakta olan cihazlar için, Intune ilkesi değerlendirilinceye kadar OOBE sırasında oluşacak Otomatik şifreleme tetiklenemez ve bu da işletim sistemi varsayılanları yerine ilke tabanlı ayarların kullanılmasına olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="3d710-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="3d710-120">S: Intune ilkesi uygulamasının bir sonucu olarak bir cihaz şifrelenmişse, bu ilke kaldırıldığında şifresi çözülür mi?</span><span class="sxs-lookup"><span data-stu-id="3d710-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="3d710-121">A: şifrelemeyle ilgili ilkenin kaldırılması, yapılandırılmış sürücülerin şifresinin çözülmesini sağlamaz.</span><span class="sxs-lookup"><span data-stu-id="3d710-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="3d710-122">S: Intune uyumluluk Ilkesinde neden aygıtımın BitLocker 'ın etkin olmadığını gösterir, ancak olsa da?</span><span class="sxs-lookup"><span data-stu-id="3d710-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="3d710-123">A: Intune uyumluluk Ilkesindeki "BitLocker etkin" ayarı Windows cihaz durumu kanıtlama (DHA) istemcisini kullanır.</span><span class="sxs-lookup"><span data-stu-id="3d710-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="3d710-124">Bu istemci yalnızca önyükleme sırasında cihaz durumunu ölçtüğünden.</span><span class="sxs-lookup"><span data-stu-id="3d710-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="3d710-125">Bu nedenle, BitLocker şifrelemesi tamamlandığından bir cihaz yeniden başlatılıncaya kadar, DHA istemci hizmeti BitLocker 'ı etkin olduğu gibi bildirmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="3d710-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 