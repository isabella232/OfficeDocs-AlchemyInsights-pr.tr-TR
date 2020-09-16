---
title: Istemci kimlik doğrulama sertifikası dağıtımında sorun giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659006"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="43ca7-102">Istemci kimlik doğrulama sertifikası dağıtımında sorun giderme</span><span class="sxs-lookup"><span data-stu-id="43ca7-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="43ca7-103">Intune NDES/SCEP ve PKCS/PFX Istemci sertifikaları profilleri, kullanıcıların şirket kaynaklarını doğrulamasına olanak tanımak için WiFi, VPN ve e-posta gibi diğer profil türleriyle birlikte yaygın olarak kullanılır.</span><span class="sxs-lookup"><span data-stu-id="43ca7-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="43ca7-104">Bu profil türleri bir istemci sertifikası profiliyle bağlantılıysa, bu profilin başarılı dağıtımına bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="43ca7-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="43ca7-105">Istemci sertifikası profilinin ilk altyapı kurulumu ve ilişkili yapılandırması genellikle sorun giderme gerektirir.</span><span class="sxs-lookup"><span data-stu-id="43ca7-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="43ca7-106">Bir adım adım kılavuz için, NDES Bağlayıcısı ve sorun giderme kılavuzunun sertifika dağıtımıyla ilgili sorunları yalıtmak için, bkz:</span><span class="sxs-lookup"><span data-stu-id="43ca7-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="43ca7-107">Intune ile SCEP desteği için altyapıyı yapılandırma</span><span class="sxs-lookup"><span data-stu-id="43ca7-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="43ca7-108">Microsoft Intune ile SCEP sertifika profillerinde sorun gidermeye genel bakış</span><span class="sxs-lookup"><span data-stu-id="43ca7-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="43ca7-109">Yapılandırmanızı doğrulamaya yardımcı olması için başvurulan PowerShell betiklerini kullanın.</span><span class="sxs-lookup"><span data-stu-id="43ca7-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="43ca7-110">Daha fazla bilgi için bkz: [Intune sertifika Bağlayıcısı doğrulama komut dosyaları](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="43ca7-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="43ca7-111">**Diğer yaygın sorunlar**</span><span class="sxs-lookup"><span data-stu-id="43ca7-111">**Other common issues**</span></span>

<span data-ttu-id="43ca7-112">**NDES Connector sunucusuna Intune sertifika bağlayıcısını yüklemeye çalıştığımda, "sertifika isteğindeki parola doğrulanamıyor" iletisi alıyorum. Zaten kullanılmış olabilir. Bu istekle göndermek için yeni bir parola alın. "**</span><span class="sxs-lookup"><span data-stu-id="43ca7-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="43ca7-113">Bu ileti, sertifika Bağlayıcısı yüklemesini yönetici olarak çalıştırmanız gerektiği anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="43ca7-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="43ca7-114">Bazı ortamlarda Intune sertifikasının çalıştığı sunucular Intune 'a bağlanmak için bir ara sunucu kullanmalıdır ve böylece sertifika bağlayıcısının bir proxy kullanması gerekir.</span><span class="sxs-lookup"><span data-stu-id="43ca7-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="43ca7-115">Bazı durumlarda, NDES Bağlayıcısı yapılandırılmış proxy ayarlarını yoksayar ve LocalSystem güvenlik bağlamında çalışırken proxy ayarlarını yapılandırmak gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="43ca7-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="43ca7-116">Çözüm, Internet Explorer 'ı SISTEM olarak çalıştırmak ve IE 'de bir proxy yapılandırmaktır.</span><span class="sxs-lookup"><span data-stu-id="43ca7-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="43ca7-117">Intune bağlayıcı hizmeti yeniden başlatıldıktan sonra, NDES Bağlayıcısı Intune 'a bağlanır.</span><span class="sxs-lookup"><span data-stu-id="43ca7-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="43ca7-118">**Kullanıcı cihazları artık NDES 'den SCEP sertifikası almıyor.**</span><span class="sxs-lookup"><span data-stu-id="43ca7-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="43ca7-119">NDES sunucusuna verilen ve NDES Bağlayıcısı yüklemesi sırasında belirtilen Istemci kimlik doğrulama sertifikasının süresi dolmuş veya yok olabilir.</span><span class="sxs-lookup"><span data-stu-id="43ca7-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="43ca7-120">Çözmek için:</span><span class="sxs-lookup"><span data-stu-id="43ca7-120">To resolve:</span></span> 
 
1. <span data-ttu-id="43ca7-121">NDES bağlayıcısını kaldırın.</span><span class="sxs-lookup"><span data-stu-id="43ca7-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="43ca7-122">Yeni bir istemci kimlik doğrulaması veya sunucu kimlik doğrulama sertifikası istemek için bu ayrıntıları kullanın:</span><span class="sxs-lookup"><span data-stu-id="43ca7-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="43ca7-123">Konu adı: CN = dış FQDN</span><span class="sxs-lookup"><span data-stu-id="43ca7-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="43ca7-124">Konu alternatif adı (ikisi de gereklidir): DNS = dış FQDN, DNS = iç FQDN</span><span class="sxs-lookup"><span data-stu-id="43ca7-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="43ca7-125">NDES bağlayıcısını yeni sertifikayla yeniden yükleyin.</span><span class="sxs-lookup"><span data-stu-id="43ca7-125">Reinstall the NDES connector with the new certificate.</span></span>