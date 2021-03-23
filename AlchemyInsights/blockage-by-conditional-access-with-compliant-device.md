---
title: Uyumlu bir cihazla Koşullu Erişim tarafından engellendim
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037080"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a><span data-ttu-id="6f42c-102">Uyumlu cihazla Koşullu Erişim tarafından engellendim</span><span class="sxs-lookup"><span data-stu-id="6f42c-102">I’m getting blocked by Conditional Access with compliant device</span></span>

<span data-ttu-id="6f42c-103">**Kesinlikle Önerilen Araçlar**</span><span class="sxs-lookup"><span data-stu-id="6f42c-103">**Highly Recommended Tools**</span></span>

- <span data-ttu-id="6f42c-104">[Cihaz Kayıt Sorun Giderici Aracı](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - En yaygın cihaz kayıt sorunlarını gidermeye yardımcı olan kapsamlı bir araçtır.</span><span class="sxs-lookup"><span data-stu-id="6f42c-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - A comprehensive tool that helps troubleshoot the most common device registration issues.</span></span>
- <span data-ttu-id="6f42c-105">[Cihaz Kayıt Bağlantısını Test Edin](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) betiği - Bir cihazın sistem hesabı altındaki Cihaz Kaydı uç noktalarına erişe olduğundan emin olmak için kullanılan bir araç.</span><span class="sxs-lookup"><span data-stu-id="6f42c-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - A tool used to ensure that a device can access Device Registration endpoints under the system account.</span></span>
- <span data-ttu-id="6f42c-106">[Azure AD Cihaz Temizleme Betiği](https://github.com/mzmaili/AzureADDeviceCleanup) - Ortamınıza eski cihazları aramak ve yönetmek için kullanılan bir araçtır.</span><span class="sxs-lookup"><span data-stu-id="6f42c-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - A tool used to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="6f42c-107">Koşullu **Erişim'in** uyumlu bir cihaz için başarısız olması veya kullanıcılarınızı neden alıyor olabilir? Kuruluş kaynağına oturum açma isteği sırasında bu iletiden ulaşamayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6f42c-107">Here are some common reasons why Conditional Access may be failing for a compliant device or why your users may be receiving **You can't get there from here** message during a sign-in request to an organizational resource.</span></span>

1. <span data-ttu-id="6f42c-108">**Cihaz, MDM'ye sahip gerekli bir cihaz durumuna sahip değil:**</span><span class="sxs-lookup"><span data-stu-id="6f42c-108">**Device is not in a required device state with an MDM**:</span></span>

<span data-ttu-id="6f42c-109">Cihazın Intune gibi onaylı bir MDM sağlayıcısına kaydedilip uyumlu *olarak işaretlenir.*</span><span class="sxs-lookup"><span data-stu-id="6f42c-109">Validate that the device is enrolled with an approved MDM provider like Intune and *marked as compliant*.</span></span> <span data-ttu-id="6f42c-110">Intune hakkında daha fazla bilgi için bu belgeye [bakın.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)</span><span class="sxs-lookup"><span data-stu-id="6f42c-110">For more information on Intune see this [document](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment).</span></span> <span data-ttu-id="6f42c-111">Cihaz uyumluluğunu ve Intune'i daha iyi anlamak için, [Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)ile yönettikleri cihazlar için kurallar ayarlamak üzere uyumluluk ilkesi kullanma.</span><span class="sxs-lookup"><span data-stu-id="6f42c-111">For better understanding of device compliance and Intune, see [use compliance policy to set rules for devices you manage with Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started).</span></span> <span data-ttu-id="6f42c-112">Bir cihazı Intune'a kaydetmede sorun giderme sorunlarıyla karşılaşılan sorunları gidermek için Microsoft'ta Cihaz kaydı sorunlarını [giderme makalesinde bulabilirsiniz.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="6f42c-112">If you are having issues enrolling a device with Intune, find troubleshooting details at [Troubleshoot device enrollment in Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span> <span data-ttu-id="6f42c-113">Daha fazla Intune desteği için bir destek isteği oluşturun.</span><span class="sxs-lookup"><span data-stu-id="6f42c-113">For further Intune support, create a support request.</span></span> <span data-ttu-id="6f42c-114">Bunu yapmak için [Intune Yardım ve Destek sayfasını ziyaret edin.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)</span><span class="sxs-lookup"><span data-stu-id="6f42c-114">To do so, visit the [Intune Help and Support page](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).</span></span>

2. <span data-ttu-id="6f42c-115">**Cihaz kuruluşlar ağına katılmadı:**</span><span class="sxs-lookup"><span data-stu-id="6f42c-115">**Device is not joined to the organizations network**:</span></span>

<span data-ttu-id="6f42c-116">Kuruluş kaynaklarına erişim için cihazın doğrudan bağlantı veya sanal özel ağ (VPN) aracılığıyla ve ayrıca şirket içi veya Azure Active Directory'ye katılmış olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="6f42c-116">For access to organizational resources, the device has to be connected to the organization's network, either through direct connection or a virtual private network (VPN), and also joined to on-premise or Azure Active Directory.</span></span> <span data-ttu-id="6f42c-117">İş cihazına kuruluş ağına katılmak için [bkz. İş cihazınızın kuruluş ağına katılma.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network)</span><span class="sxs-lookup"><span data-stu-id="6f42c-117">To join a work device to the organization network, see [Join your work device to your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network).</span></span> <span data-ttu-id="6f42c-118">Kişisel/TEKM cihazı kaydetmek için bkz. Kişisel [cihazınızı kurum ağınıza kaydetme.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)</span><span class="sxs-lookup"><span data-stu-id="6f42c-118">To register a personal/BYOD device, see [Register your personal device on your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).</span></span>

- <span data-ttu-id="6f42c-119">Cihazın ağa katıldığını doğrulamak için, buradaki kayıtlı cihazların veya iş [cihazlarının](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) adımlarını takip [edebilirsiniz.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined)</span><span class="sxs-lookup"><span data-stu-id="6f42c-119">To validate whether the device has joined the network, you can follow the steps for registered devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) or work devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined).</span></span> <span data-ttu-id="6f42c-120">Sorunu Kuruluş ağı bağlantısı kapsamında yapmak için aşağıdaki yönergeleri izleyin:</span><span class="sxs-lookup"><span data-stu-id="6f42c-120">To scope the issue to Org network connectivity, follow guidelines below:</span></span>

    1. <span data-ttu-id="6f42c-121">örneğin iş veya okul hesabınızla Windows'ta oturum alain@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="6f42c-121">Sign in to Windows using your work or school account,  for example, alain@contoso.com.</span></span>
    2. <span data-ttu-id="6f42c-122">Vpn veya DirectAccess aracılığıyla kuruluş ağınıza bağlanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6f42c-122">Connect to your organization's network through a VPN or DirectAccess.</span></span>
    3. <span data-ttu-id="6f42c-123">Bağlandıktan sonra cihazınızı kilitlemek için **Windows logo tuşu+L** tuşlarına basın.</span><span class="sxs-lookup"><span data-stu-id="6f42c-123">After you're connected, press the **Windows logo key+L** to lock your device.</span></span>
    4. <span data-ttu-id="6f42c-124">İş veya okul hesabınızla cihazınızın kilidini açın ve sorunlu uygulama veya hizmete yeniden erişmeyi deneyin.</span><span class="sxs-lookup"><span data-stu-id="6f42c-124">Unlock your device using your work or school account, and then try to access the problematic app or service again.</span></span>

<span data-ttu-id="6f42c-125">Buradan buraya **tekrar gelemedi hata iletisini görüyorsanız,** sorun muhtemelen başka bir yerdedir.</span><span class="sxs-lookup"><span data-stu-id="6f42c-125">If you see the **You can't get there from here** error message again, issue is likely elsewhere.</span></span>

3. <span data-ttu-id="6f42c-126">**İşletim sistemi desteklenmiyor:**</span><span class="sxs-lookup"><span data-stu-id="6f42c-126">**Operating system is not supported**:</span></span>

<span data-ttu-id="6f42c-127">İşletim sisteminin desteklenen bir sürümünü çalıştırmış olduğundan emin olun; aşağıdakiler de dahil:</span><span class="sxs-lookup"><span data-stu-id="6f42c-127">Ensure that you're running a supported version of the operating system, including:</span></span>

- <span data-ttu-id="6f42c-128">**Windows İstemcisi:** Windows 7 veya sonrası</span><span class="sxs-lookup"><span data-stu-id="6f42c-128">**Windows Client**: Windows 7 or later</span></span>

- <span data-ttu-id="6f42c-129">**Windows Server**: Windows Server 2008 R2 veya sonrası</span><span class="sxs-lookup"><span data-stu-id="6f42c-129">**Windows Server**: Windows Server 2008 R2 or later</span></span>

- <span data-ttu-id="6f42c-130">**macOS**: macOS X veya sonrası</span><span class="sxs-lookup"><span data-stu-id="6f42c-130">**macOS**: macOS X or later</span></span>

- <span data-ttu-id="6f42c-131">**Android ve iOS**: Android ve iOS mobil işletim sistemlerinin en son sürümü</span><span class="sxs-lookup"><span data-stu-id="6f42c-131">**Android and iOS**: Latest version of Android and iOS mobile operating systems</span></span>

4. <span data-ttu-id="6f42c-132">**Web tarayıcısı desteklenmiyor:**</span><span class="sxs-lookup"><span data-stu-id="6f42c-132">**Web browser is not supported**:</span></span>

<span data-ttu-id="6f42c-133">Lütfen aşağıdaki desteklenen tarayıcıları bulun.</span><span class="sxs-lookup"><span data-stu-id="6f42c-133">Please find supported browsers below.</span></span> <span data-ttu-id="6f42c-134">Windows 1703 veya sonraki sürümlerde Chrome desteği için Windows 10 Hesapları uzantısı gereklidir.</span><span class="sxs-lookup"><span data-stu-id="6f42c-134">For Chrome support with Windows 1703 or later versions, a Windows 10 Accounts extension is required.</span></span> <span data-ttu-id="6f42c-135">Edge 85+ için, cihaz uyumluluk bilgilerini düzgün bir şekilde geçmek için kullanıcının oturumlarının açık olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="6f42c-135">For Edge 85+, the user needs to be signed in to properly pass device compliance information.</span></span> <span data-ttu-id="6f42c-136">Diğer ayrıntılar için buraya [bakın.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)</span><span class="sxs-lookup"><span data-stu-id="6f42c-136">For more details, see [here](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

- <span data-ttu-id="6f42c-137">**Windows 10**: Microsoft Edge, Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="6f42c-137">**Windows 10**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="6f42c-138">**Windows 8 / 8.1**: Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="6f42c-138">**Windows 8 / 8.1**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="6f42c-139">**Windows 7**: Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="6f42c-139">**Windows 7**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="6f42c-140">**iOS**: Microsoft Edge, Intune Yönetilen Tarayıcısı, Safari</span><span class="sxs-lookup"><span data-stu-id="6f42c-140">**iOS**: Microsoft Edge, Intune Managed Browser, Safari</span></span>
- <span data-ttu-id="6f42c-141">**Android**: **Microsoft Edge**: Intune Yönetilen Tarayıcı, Chrome</span><span class="sxs-lookup"><span data-stu-id="6f42c-141">**Android**: **Microsoft Edge**: Intune Managed Browser, Chrome</span></span>
- <span data-ttu-id="6f42c-142">**Windows Phone**: Microsoft Edge, Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="6f42c-142">**Windows Phone**: Microsoft Edge, Internet Explorer</span></span>
- <span data-ttu-id="6f42c-143">**Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="6f42c-143">**Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="6f42c-144">**Windows Server 2016**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="6f42c-144">**Windows Server 2016**: Internet Explorer</span></span>
- <span data-ttu-id="6f42c-145">**Windows Server 2012 R2**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="6f42c-145">**Windows Server 2012 R2**: Internet Explorer</span></span>
- <span data-ttu-id="6f42c-146">**Windows Server 2008 R2**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="6f42c-146">**Windows Server 2008 R2**: Internet Explorer</span></span>
- <span data-ttu-id="6f42c-147">**macOS**: Chrome, Safari</span><span class="sxs-lookup"><span data-stu-id="6f42c-147">**macOS**: Chrome, Safari</span></span>

<span data-ttu-id="6f42c-148">Daha fazla bilgi için **buraya ileti ve sorun giderme** adımlarını buradan [edinebilirsiniz.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)</span><span class="sxs-lookup"><span data-stu-id="6f42c-148">Find more information on the **You can't get there** message and troubleshooting steps [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).</span></span>
