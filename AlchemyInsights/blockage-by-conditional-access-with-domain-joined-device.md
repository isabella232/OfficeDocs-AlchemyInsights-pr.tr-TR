---
title: Etki alanına katılmış bir cihazla Koşullu Erişim tarafından engellendim
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038106"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="e88da-102">Etki alanına katılmış bir cihazla Koşullu Erişim tarafından engellendim</span><span class="sxs-lookup"><span data-stu-id="e88da-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="e88da-103">**Kesinlikle Önerilen Araçlar**</span><span class="sxs-lookup"><span data-stu-id="e88da-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="e88da-104">[Cihaz Kayıt Sorun Giderici Aracı](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - En yaygın cihaz kayıt sorunlarını gidermeye yardımcı olan araçtır.</span><span class="sxs-lookup"><span data-stu-id="e88da-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="e88da-105">[Cihaz Kayıt Bağlantısı betiği-](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) Bir cihazın sistem hesabı altındaki Cihaz Kaydı uç noktalarına erişemelerini sağlamaya yardımcı olan betik.</span><span class="sxs-lookup"><span data-stu-id="e88da-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="e88da-106">[Azure AD Cihaz Temizleme Betiği](https://github.com/mzmaili/AzureADDeviceCleanup) - Ortamınıza eski cihazları aramanızı ve yönetmenizi sağlayan betik.</span><span class="sxs-lookup"><span data-stu-id="e88da-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="e88da-107">İşte koşullu erişimin etki alanına (Karma Azure AD) katılmış bir cihazda başarısız olmasıyla ilgili bazı yaygın nedenler.</span><span class="sxs-lookup"><span data-stu-id="e88da-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="e88da-108">**Cihazda Azure AD PRT** yoktur. Cihazın Azure AD Birincil Yenileme Belirteci'ne (PRT) sahip olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="e88da-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="e88da-109">PRT hakkında daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="e88da-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="e88da-110">Azure AD PRT'niz olup olduğunu doğrulamak için, cihazda komutu çalıştırabilirsiniz ve `dsregcmd/status` "AzureAdPrt" eşittir "EVET".</span><span class="sxs-lookup"><span data-stu-id="e88da-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="e88da-111">"AzureAdPrt" "HAYıR" ise, şunları kontrol edin:</span><span class="sxs-lookup"><span data-stu-id="e88da-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="e88da-112">**AD FS ile** bir federasyon ortamınız olup olmadığı ve bu ortam kullanıcılarının ev ağlarından erişilemiyor olabilir: Bu durumda, "kullanıcıadı"sı olan" uç noktalarınıza extranet'den erişile olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="e88da-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="e88da-113">AD FS'niz bir VPN'nin arkasında ise, kullanıcıların VPN'ye bağlana olduğundan emin olun ve cihaza yeniden oturum açın.</span><span class="sxs-lookup"><span data-stu-id="e88da-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="e88da-114">Daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)</span><span class="sxs-lookup"><span data-stu-id="e88da-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="e88da-115">**Cihazın TPM'sinde** hata olup olmadığı ve dolayısıyla cihazın kimliğini doğrulayama durumunun doğrulanıp doğrulanamayıp doğrulanamama: TPM durumunun "Hazır" olup olmadığını görmek için "tpm.msc"yi kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="e88da-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="e88da-116">Yoksa, çalıştırın `dsregcmd/leave` ve cihazın Azure AD'ye yeniden katılmasına izin verme.</span><span class="sxs-lookup"><span data-stu-id="e88da-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="e88da-117">Daha sonra yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="e88da-117">Then, try again.</span></span> <span data-ttu-id="e88da-118">Daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="e88da-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="e88da-119">**Üçüncü taraf bir kimlik sağlayıcısı kullanıyorsanız ve bu** sağlayıcı üçüncü taraf kimlik WS-Trust desteklemez.</span><span class="sxs-lookup"><span data-stu-id="e88da-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="e88da-120">Belgelerimizde açıklandığı gibi, Azure AD'ye katılmış karma cihazlar bu durumda çalışamaz.</span><span class="sxs-lookup"><span data-stu-id="e88da-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="e88da-121">Destek için lütfen Kimlik sağlayıcınızla birlikte çalışabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e88da-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="e88da-122">**Windows 10** Hesapları veya Office uzantısı olmadan kullanıcılar Chrome tarayıcısını **kullanıyorsa Chrome, AAD'ye** katılmış veya karma AAD'ye katılmış cihazlarda PRT'yi otomatik olarak kullanmaz: Bu, "Kayıtsız cihaz" hata iletisi görüntülendiğinde cihaz tabanlı Koşullu Erişim ilkelerinin başarısızlığına yol açabilir.</span><span class="sxs-lookup"><span data-stu-id="e88da-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="e88da-123">Chrome tarayıcısını doğru kullanmak için SCCM veya Intune aracılığıyla "Windows 10 Hesapları" veya "Kullanıcıların Chrome tarayıcısına Office uzantısını" yüklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="e88da-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="e88da-124">Daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)</span><span class="sxs-lookup"><span data-stu-id="e88da-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="e88da-125">Uzantıyı uzaktan itmek mümkün yoksa, cihaz tabanlı Koşullu Erişim'in arkasındaki uygulamalara erişmek için kullanıcılara yukarıdaki uzantılardan birini el ile yüklemelerini bildirin.</span><span class="sxs-lookup"><span data-stu-id="e88da-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="e88da-126">Daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)</span><span class="sxs-lookup"><span data-stu-id="e88da-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="e88da-127">Cihaz Azure AD'ye doğru bir şekilde katılmış, ancak Azure AD Connect'te yapılan eşitleme değişiklikleri veya **Azure portalında** yapılan eşitleme değişiklikleri nedeniyle yanlışlıkla silinmiş veya devre dışı bırakılmış olabilir: Böyle bir durumda, "AzureAdJoined" ve "PRT" durumu cihazda geçerli olarak gösterse bile cihaz nesnesi artık tam olarak katılmış bir cihaz olarak tanınmıyor.</span><span class="sxs-lookup"><span data-stu-id="e88da-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="e88da-128">Bu sorunu çözmek için, `dsregcmd/leave` etkilenen cihazlarda çalıştırın ve Azure AD'ye yeniden katılmalarına izin ver.</span><span class="sxs-lookup"><span data-stu-id="e88da-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="e88da-129">Daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)</span><span class="sxs-lookup"><span data-stu-id="e88da-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="e88da-130">Cihazlarınız Windows 10 1809 güncelleştirmesinde, VPN/Bulut Proxy'si ile çalışıyor ve "AzureAdPrt" durumu veya SSO sorunu olan herhangi bir uygulamayla ilgili sorunları görüyorsanız (PRT'niz olsa bile outlook posta kutusuna bağlanıyorsa), bu makinelerde PRT hatalarını önlemek için [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) veya Nisan toplu güncelleştirmesi [KB4549949'u](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) gördüğünüzden emin olun.</span><span class="sxs-lookup"><span data-stu-id="e88da-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















