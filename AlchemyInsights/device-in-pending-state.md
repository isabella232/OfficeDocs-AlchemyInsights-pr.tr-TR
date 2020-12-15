---
title: Bekleme durumunda cihaz
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679995"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="e9e76-102">Bekleme durumunda cihaz</span><span class="sxs-lookup"><span data-stu-id="e9e76-102">Device in pending state</span></span>

<span data-ttu-id="e9e76-103">**Koşullar**</span><span class="sxs-lookup"><span data-stu-id="e9e76-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="e9e76-104">Cihaz kayıtlarını ilk kez ayarlıyorsanız, Azure AD 'nın altındaki cihazları nasıl edindiğinize yol gösterecek olan [Azure Active Directory 'de (Azure AD) cihaz yönetimine giriş](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) konusunda gözden geçirdiğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="e9e76-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="e9e76-105">Cihazları Azure AD 'ye doğrudan kaydedip Intune 'a kaydettirirken, [Intune 'u yapılandırdığınızdan](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ve öncelikle [Lisans](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) 'ı kullandığınızdan emin olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="e9e76-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="e9e76-106">Azure AD ve şirket içi AD 'de işlemleri gerçekleştirme yetkiniz olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="e9e76-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="e9e76-107">Yalnızca Azure AD 'deki genel yönetici, cihaz kayıtlarında ayarları yönetebilir.</span><span class="sxs-lookup"><span data-stu-id="e9e76-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="e9e76-108">Ayrıca, şirket içi Active Directory 'nizde otomatik kayıtları ayarlıyorsanız, Active Directory ve AD FS yöneticisi olmanız gerekir (uygulanabiliyorsa).</span><span class="sxs-lookup"><span data-stu-id="e9e76-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="e9e76-109">Karma Azure AD katılma kayıt süreci, aygıtların şirket ağında olmasını gerektirir.</span><span class="sxs-lookup"><span data-stu-id="e9e76-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="e9e76-110">Ayrıca VPN üzerinden de çalışır, ancak bazı uyarılar vardır.</span><span class="sxs-lookup"><span data-stu-id="e9e76-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="e9e76-111">Uzaktan çalışma durumları altında karma Azure AD katılma kaydı işlemini sorun giderme konusunda yardım almak için müşteriler duyduk.</span><span class="sxs-lookup"><span data-stu-id="e9e76-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="e9e76-112">**Bulut kimlik doğrulama ortamı (Azure AD parola karma eşitleme veya geçiş kimlik doğrulaması kullanılarak)**</span><span class="sxs-lookup"><span data-stu-id="e9e76-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="e9e76-113">Bu kayıt akışı, "eşitleme katılma" olarak da bilinir.</span><span class="sxs-lookup"><span data-stu-id="e9e76-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="e9e76-114">Kayıt işlemi sırasında neler olduğunu aşağıda bulabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="e9e76-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="e9e76-115">Windows 10, Kullanıcı cihazda oturum açtığında hizmet bağlantı noktası (SCP) kaydını bulur.</span><span class="sxs-lookup"><span data-stu-id="e9e76-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="e9e76-116">Cihaz öncelikle kayıt defterinde (HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD], istemci tarafı SCP 'den kiracı bilgilerini almaya çalışır.</span><span class="sxs-lookup"><span data-stu-id="e9e76-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="e9e76-117">Daha fazla bilgi için bkz [.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)</span><span class="sxs-lookup"><span data-stu-id="e9e76-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="e9e76-118">Başarısız olursa, cihaz SCP 'den kiracı bilgilerini almak için şirket içi Active Directory ile iletişim kurar.</span><span class="sxs-lookup"><span data-stu-id="e9e76-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="e9e76-119">SCP 'yi doğrulamak için bu [belgeye](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)başvurun.</span><span class="sxs-lookup"><span data-stu-id="e9e76-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="e9e76-120">Active Directory 'de SCP 'YI etkinleştirmeyi ve yalnızca istemci tarafı SCP 'YI ilk doğrulama için kullanmayı öneririz.</span><span class="sxs-lookup"><span data-stu-id="e9e76-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="e9e76-121">Windows 10, sistem bağlamı altındaki Azure AD ile iletişim kurmaya çalışır.</span><span class="sxs-lookup"><span data-stu-id="e9e76-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="e9e76-122">Cihazın sistem hesabı altındaki Microsoft kaynaklarına erişip erişebildiğini, [test cihazı kayıt bağlantı betiğini](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)kullanarak doğrulayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e9e76-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="e9e76-123">Windows 10 kendinden imzalanan sertifika oluşturur ve şirket içi Active Directory 'de bilgisayar nesnesinin altında depolar.</span><span class="sxs-lookup"><span data-stu-id="e9e76-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="e9e76-124">Bu, etki alanı denetleyicisine görüntülenecek satır gerektirir.</span><span class="sxs-lookup"><span data-stu-id="e9e76-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="e9e76-125">Sertifikası olan cihaz nesnesi Azure AD Connect aracılığıyla Azure AD ile eşitlenir.</span><span class="sxs-lookup"><span data-stu-id="e9e76-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="e9e76-126">Eşitleme döngüyü varsayılan olarak her 30 dakikada bir, ancak Azure AD Connect 'in yapılandırmasına bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="e9e76-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="e9e76-127">Daha fazla bilgi için bu [belgeye](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)bakın.</span><span class="sxs-lookup"><span data-stu-id="e9e76-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="e9e76-128">Bu aşamada, konu aygıtını Azure portalının cihaz Blade altında "**Beklemede**" durumunda görebilmelisiniz.</span><span class="sxs-lookup"><span data-stu-id="e9e76-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="e9e76-129">Windows 10 ' da sonraki kullanıcı oturumunda, kayıt tamamlanmış olacaktır.</span><span class="sxs-lookup"><span data-stu-id="e9e76-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e9e76-130">VPN kullanıyorsanız ve oturum kapatma/oturum açma/oturum açma</span><span class="sxs-lookup"><span data-stu-id="e9e76-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="e9e76-131">Bunu yapmak için:</span><span class="sxs-lookup"><span data-stu-id="e9e76-131">To do that:</span></span>
    >
    > <span data-ttu-id="e9e76-132">`dsregcmd /join`Yönetici isteminde ya da bilgisayarınıza PSExec aracılığıyla uzaktan sorun.</span><span class="sxs-lookup"><span data-stu-id="e9e76-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="e9e76-133">Örneğin: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="e9e76-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="e9e76-134">Azure Active Directory cihaz kaydıyla ilgili yaygın sorunlar için, [CIHAZLAR SSS](https://docs.microsoft.com/azure/active-directory/devices/faq)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="e9e76-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
