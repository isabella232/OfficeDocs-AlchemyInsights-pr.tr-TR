---
title: Stok sorununu giderme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573904"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="37b52-102">Stok sorununu giderme</span><span class="sxs-lookup"><span data-stu-id="37b52-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="37b52-103">Herhangi bir cihazın kimliği doğrulanmış almayı tamamlamak için, tam olarak kaydedilmelidir ve iyi bir durumda ve birincil yenileme belirteci (PRT) edinebilmek gerekir.</span><span class="sxs-lookup"><span data-stu-id="37b52-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="37b52-104">Karma Azure AD katılma kayıt süreci, aygıtların şirket ağında olmasını gerektirir.</span><span class="sxs-lookup"><span data-stu-id="37b52-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="37b52-105">Ayrıca VPN üzerinden de çalışır, ancak bazı uyarılar vardır.</span><span class="sxs-lookup"><span data-stu-id="37b52-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="37b52-106">Uzaktan çalışma durumları altında karma Azure AD katılma kaydını sorun giderme konusunda yardım almak için müşteriler olduğunu duyduk.</span><span class="sxs-lookup"><span data-stu-id="37b52-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="37b52-107">İşte, kayıt işlemi sırasında "çok yer</span><span class="sxs-lookup"><span data-stu-id="37b52-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="37b52-108">**Bulut kimlik doğrulama ortamı (Azure AD parola karma eşitleme veya geçiş kimlik doğrulaması kullanılarak)**</span><span class="sxs-lookup"><span data-stu-id="37b52-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="37b52-109">Bu kayıt akışı, "eşitleme katılma" olarak da bilinir.</span><span class="sxs-lookup"><span data-stu-id="37b52-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="37b52-110">Windows 10, kullanıcının cihazda oturum açarken bir SCP kaydını bulur.</span><span class="sxs-lookup"><span data-stu-id="37b52-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="37b52-111">Cihaz öncelikle kayıt defterinde (HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD], istemci tarafı SCP 'den kiracı bilgilerini almaya çalışır.</span><span class="sxs-lookup"><span data-stu-id="37b52-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="37b52-112">Daha fazla bilgi için bu [belgeye](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)bakın.</span><span class="sxs-lookup"><span data-stu-id="37b52-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="37b52-113">Başarısız olursa, cihaz hizmet bağlantı noktasından (SCP) kiracı bilgilerini almak için şirket içi Active Directory (AD) ile iletişim kurar.</span><span class="sxs-lookup"><span data-stu-id="37b52-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="37b52-114">SCP 'yi doğrulamak için lütfen bu [belgeye](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)başvurun.</span><span class="sxs-lookup"><span data-stu-id="37b52-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="37b52-115">İlk doğrulama için AD içinde SCP 'YI etkinleştirip yalnızca istemci tarafı SCP 'YI kullanmayı öneririz.</span><span class="sxs-lookup"><span data-stu-id="37b52-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="37b52-116">Windows 10, sistem bağlamı altındaki Azure AD ile iletişim kurmaya çalışır.</span><span class="sxs-lookup"><span data-stu-id="37b52-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="37b52-117">Cihazın sistem hesabı altındaki Microsoft kaynaklarına erişip erişebildiğini, test cihazı kayıt bağlantı betiğini kullanarak doğrulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="37b52-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="37b52-118">Windows 10 kendinden imzalanan bir sertifika oluşturur ve şirket içi AD 'de bilgisayar nesnesinin altında depolar.</span><span class="sxs-lookup"><span data-stu-id="37b52-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="37b52-119">Bu, etki alanı denetleyicisine görüntülenecek satır gerektirir.</span><span class="sxs-lookup"><span data-stu-id="37b52-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="37b52-120">Azure AD Connect aracılığıyla, sertifikaya sahip bir cihaz nesnesi Azure AD ile eşitlenmiş.</span><span class="sxs-lookup"><span data-stu-id="37b52-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="37b52-121">Eşitleme döngüyü varsayılan olarak her 30 dakikada bir, ancak Azure AD Connect 'in yapılandırmasına bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="37b52-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="37b52-122">Daha fazla bilgi için lütfen bu [belgeye](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)bakın.</span><span class="sxs-lookup"><span data-stu-id="37b52-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="37b52-123">Bu aşamada, konu aygıtını Azure portalının cihaz Blade altında "beklemede" durumunda görebilmelisiniz.</span><span class="sxs-lookup"><span data-stu-id="37b52-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="37b52-124">Windows 10 ' da sonraki kullanıcı oturumunda, kayıt tamamlanmış olacaktır.</span><span class="sxs-lookup"><span data-stu-id="37b52-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="37b52-125">VPN kullanıyorsanız ve oturum kapatma işlemini etki alanı bağlantısını sona erdirirse, kaydı el ile tetikleyebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="37b52-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="37b52-126">Bir dsregcmd/Join 'i yerel olarak yönetici isteminde veya PSExec aracılığıyla PC 'nize uzaktan yapın.</span><span class="sxs-lookup"><span data-stu-id="37b52-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="37b52-127">Örneğin, PsExec-s \\ win10client01 cmd, dsregcmd/Join</span><span class="sxs-lookup"><span data-stu-id="37b52-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="37b52-128">Karma birleşim [sorunlarıyla ilgili daha](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="37b52-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
