---
title: VPN ile ilgili sorunlar
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555742"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="d76bd-102">VPN ile ilgili sorunlar</span><span class="sxs-lookup"><span data-stu-id="d76bd-102">VPN related issues</span></span>

<span data-ttu-id="d76bd-103">MDM istemcileri için VPN bağlantısının başarılı bir şekilde uygulanması, VPN altyapısının gereksinimlerini doğru şekilde yansıtan dağıtılmış bir profile bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="d76bd-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="d76bd-104">Araştırdığınız istemci platformları için uygun ayarlar için bkz:</span><span class="sxs-lookup"><span data-stu-id="d76bd-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="d76bd-105">Intune kullanarak VPN bağlantıları eklemek için Windows 10 ve Windows Holografik cihaz ayarları</span><span class="sxs-lookup"><span data-stu-id="d76bd-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="d76bd-106">Microsoft Intune'da iOS ve iPadOS aygıtlarında VPN ayarları ekleme</span><span class="sxs-lookup"><span data-stu-id="d76bd-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="d76bd-107">Intune VPN yapılandırmak için Android cihaz ayarları</span><span class="sxs-lookup"><span data-stu-id="d76bd-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="d76bd-108">Microsoft Intune'daki macOS aygıtlarında VPN ayarları ekleme</span><span class="sxs-lookup"><span data-stu-id="d76bd-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="d76bd-109">VPN profiliniz sertifika tabanlı kimlik doğrulaması kullanıyorsa, VPN profiline bağlı kök sertifika ve istemci kimlik doğrulama sertifikası profillerinin başarıyla dağıtıldıklarından emin olun.</span><span class="sxs-lookup"><span data-stu-id="d76bd-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="d76bd-110">**Sık Karşılaşılan Sorunlar**</span><span class="sxs-lookup"><span data-stu-id="d76bd-110">**Common Issues**</span></span>

<span data-ttu-id="d76bd-111">**Bir cihaza VPN profili dağıttım. Intune başarılı olduğunu gösteriyor, ancak cihaz VPN'e bağlanmıyor.**</span><span class="sxs-lookup"><span data-stu-id="d76bd-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="d76bd-112">Başarılı bir durum, Intune'un profili yapılandırılmış olarak başarıyla dağıtmış olduğu anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="d76bd-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="d76bd-113">Ancak, bu yapılandırmalar ağınız ve/veya kimlik doğrulama gereksinimleriniz ile eşleşmeyebilir.</span><span class="sxs-lookup"><span data-stu-id="d76bd-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="d76bd-114">Altyapı ve kimlik doğrulama hizmetindeki günlükleri (VPN sunucusunda ve NPS/Radius sunucusunda) inceleyin ve bağlantı girişimi hakkında daha fazla bilgi sağlayın.</span><span class="sxs-lookup"><span data-stu-id="d76bd-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="d76bd-115">Günlükleri toplamak ve incelemek için ağ altyapı ekibiniz veya üçüncü taraf VPN satıcınızla çalışmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="d76bd-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="d76bd-116">**iOS için özel bir VPN yapılandırdığımda, uygulama başına VPN özelliği kullanıma sunulmadı.**</span><span class="sxs-lookup"><span data-stu-id="d76bd-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="d76bd-117">Intune'daki iOS aygıtları için uygulama başına VPN şu anda, uygulama başına VPN'i yapılandırmadan önce sertifika ön koşullarını karşılaması gereken belirli bir sağlayıcı lar ve iş ortakları listesi için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="d76bd-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="d76bd-118">Daha fazla bilgi için bkz: [Intune'daki iOS/iPadOS aygıtları için uygulama başına Sanal Özel Ağ (VPN) ayarlayın.](https://docs.microsoft.com/intune/vpn-setting-configure-per-app)</span><span class="sxs-lookup"><span data-stu-id="d76bd-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="d76bd-119">Intune'daki tüm VPN bağlantı türleri hakkında daha fazla bilgi için, [Intune'daki VPN sunucularına bağlanmak için VPN profilleri oluştur'a](https://docs.microsoft.com/intune/vpn-settings-configure)bakın.</span><span class="sxs-lookup"><span data-stu-id="d76bd-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="d76bd-120">**iOS İsteğe Bağlı VPN, yapılandırılmış bir etki alanına erişildiğinde tetiklenmiyor**</span><span class="sxs-lookup"><span data-stu-id="d76bd-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="d76bd-121">Otomatik VPN ayarlarını test etmek için aşağıdaki değerleri ayarlayın:</span><span class="sxs-lookup"><span data-stu-id="d76bd-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="d76bd-122">Aşağıdakileri yapmak istiyorum: **Her bağlantı girişimini değerlendirin**</span><span class="sxs-lookup"><span data-stu-id="d76bd-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="d76bd-123">Bağlanıp bağlanmayın: **Gerekirse bağlanın**</span><span class="sxs-lookup"><span data-stu-id="d76bd-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="d76bd-124">Kullanıcılar bu etki alanına erişirken: **hedef** *alan adı*</span><span class="sxs-lookup"><span data-stu-id="d76bd-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="d76bd-125">Yukarıdaki yapılandırma başarılı değilse, aşağıdaki öğeyi ekleyin:</span><span class="sxs-lookup"><span data-stu-id="d76bd-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="d76bd-126">Bu URL'ye erişimediğinde, VPN'i bağlamakuvvetine ulaşın: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="d76bd-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>