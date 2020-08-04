---
title: Sorun giderme İstemci Kimlik Doğrulama sertifika dağıtımı
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555806"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="87993-102">Sorun giderme İstemci Kimlik Doğrulama sertifika dağıtımı</span><span class="sxs-lookup"><span data-stu-id="87993-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="87993-103">Intune NDES/SCEP ve PKCS/PFX Client sertifikaları profilleri, kullanıcıların şirket kaynaklarına kimlik doğrulamasına olanak sağlamak için Wifi, VPN ve e-posta gibi diğer profil türleri ile birlikte yaygın olarak kullanılır.</span><span class="sxs-lookup"><span data-stu-id="87993-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="87993-104">Bu profil türleri bir istemci sertifikası profiline bağlandığında, bu profilin başarılı bir şekilde dağıtılmasına bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="87993-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="87993-105">İlk altyapı kurulumu ve İstemci Sertifikası profilinin ilişkili yapılandırması genellikle sorun giderme gerektirir.</span><span class="sxs-lookup"><span data-stu-id="87993-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="87993-106">SERTIFIKA dağıtımıyla ilgili sorunları yalıtmak için NDES bağlayıcısının başarılı bir şekilde kurulumu ve sorun giderme kılavuzu için adım adım kılavuz için bkz:</span><span class="sxs-lookup"><span data-stu-id="87993-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="87993-107">Intune ile SCEP'i destekleyecek altyapıyı yapılandırın</span><span class="sxs-lookup"><span data-stu-id="87993-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="87993-108">Microsoft Intune ile Sorun Giderme SCEP sertifika profillerine genel bakış</span><span class="sxs-lookup"><span data-stu-id="87993-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="87993-109">Yapılandırmanızı doğrulamaya yardımcı olmak için başvurulan powershell komut dosyalarını kullanın.</span><span class="sxs-lookup"><span data-stu-id="87993-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="87993-110">Daha fazla bilgi için [Intune Certificate bağlayıcı sıyrık doğrulama komut dosyalarına](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)bakın.</span><span class="sxs-lookup"><span data-stu-id="87993-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="87993-111">**Diğer yaygın sorunlar**</span><span class="sxs-lookup"><span data-stu-id="87993-111">**Other common issues**</span></span>

<span data-ttu-id="87993-112">**NDES bağlayıcı sunucusuna Intune sertifika bağlayıcısını yüklemeye çalıştığımda, "Sertifika isteğindeki parola doğrulanamıyor. Zaten kullanılmış olabilir. Bu istekle göndermek için yeni bir parola edinin."**</span><span class="sxs-lookup"><span data-stu-id="87993-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="87993-113">Bu ileti, sertifika bağlayıcısı yüklemesini Yönetici olarak çalıştırmanız gerektiği anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="87993-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="87993-114">Bazı ortamlarda, Intune Sertifikası'nın çalıştığı sunucuların Intune'a bağlanmak için bir proxy sunucusu kullanması ve bu nedenle Sertifika Bağlayıcısı'nın bir proxy kullanması gerekir.</span><span class="sxs-lookup"><span data-stu-id="87993-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="87993-115">Bazı durumlarda, NDES Bağlayıcısı yapılandırılan proxy ayarlarını yoksayarlar ve LocalSystem'in güvenlik bağlamında çalışırken proxy ayarlarını yapılandırmak gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="87993-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="87993-116">Çözüm System olarak Internet Explorer çalıştırmak ve IE bir proxy yapılandırmaktır.</span><span class="sxs-lookup"><span data-stu-id="87993-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="87993-117">Intune Bağlayıcı Hizmetiyeniden başladıktan sonra NDES Bağlayıcısı Intune'a bağlanır.</span><span class="sxs-lookup"><span data-stu-id="87993-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="87993-118">**Kullanıcı aygıtları artık NDES'ten SCEP sertifikaları almıyor.**</span><span class="sxs-lookup"><span data-stu-id="87993-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="87993-119">NDES sunucusuna verilen ve NDES bağlayıcıyüklemesi sırasında belirtilen İstemci Kimlik Doğrulama sertifikasının süresi dolmuş veya eksik olabilir.</span><span class="sxs-lookup"><span data-stu-id="87993-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="87993-120">Çözmek için:</span><span class="sxs-lookup"><span data-stu-id="87993-120">To resolve:</span></span> 
 
1. <span data-ttu-id="87993-121">NDES konektörünü kaldırın.</span><span class="sxs-lookup"><span data-stu-id="87993-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="87993-122">Yeni bir istemci kimlik doğrulama veya sunucu kimlik doğrulama sertifikası istemek için bu ayrıntıları kullanın:</span><span class="sxs-lookup"><span data-stu-id="87993-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="87993-123">Konu adı: CN=external fqdn</span><span class="sxs-lookup"><span data-stu-id="87993-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="87993-124">Özne alternatif adı (her ikisi de gereklidir): DNS=dış fqdn, DNS=iç fqdn</span><span class="sxs-lookup"><span data-stu-id="87993-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="87993-125">NDES konektörünü yeni sertifikayla yeniden yükleyin.</span><span class="sxs-lookup"><span data-stu-id="87993-125">Reinstall the NDES connector with the new certificate.</span></span>