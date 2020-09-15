---
title: Microsoft Intune 'da Android cihazlarını kaydetme sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689974"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="678de-102">Microsoft Intune 'da Android cihazlarını kaydetme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="678de-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="678de-103">Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="678de-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="678de-104">Bazı yaygın sorunlar ve çözüm adımları:</span><span class="sxs-lookup"><span data-stu-id="678de-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="678de-105">**Şirket portalında cihaz şifrelenmemiş hatası:** Cihazınızın tümüyle şifrelendiğinden emin olmak için, özellikle de v 7.0 ile başlayan Android 'in daha yeni sürümleri için başlangıç parolası gerekir.</span><span class="sxs-lookup"><span data-stu-id="678de-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="678de-106">Genel çözümler, başlangıç PIN 'ini etkinleştirmek veya cihazı tümüyle şifrelemektir.</span><span class="sxs-lookup"><span data-stu-id="678de-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="678de-107">Daha fazla bilgi için [Bu belgeyi](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="678de-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="678de-108">**Cihazlar Intune hizmetine iade edemeyecek veya Intune yönetim konsolunda "sağlıksız" olarak görüntülenmeyecek:** Bazı Samsung 4,4 ve 5,5 cihazları hizmeti iade edebilir.</span><span class="sxs-lookup"><span data-stu-id="678de-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="678de-109">Bu sorunun 3 olası çözümü vardır:</span><span class="sxs-lookup"><span data-stu-id="678de-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="678de-110">Cihaz eşitlemesini otomatik olarak başlatan Intune şirket portalı uygulamasını el ile açın.</span><span class="sxs-lookup"><span data-stu-id="678de-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="678de-111">Cihazı Android 6,0 veya üzeri olarak güncelleyin.</span><span class="sxs-lookup"><span data-stu-id="678de-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="678de-112">Samsung akıllı Manager 'ın Intune şirket portalını yönetmesini devre dışı bırakın.</span><span class="sxs-lookup"><span data-stu-id="678de-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="678de-113">Bu sorunlar ve çözünürlükler hakkında daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) inceleyin.</span><span class="sxs-lookup"><span data-stu-id="678de-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="678de-114">**Kullanıcı Lisans türü geçersiz** veya **Kullanıcı adı tanınmadı hata:** kullanıcıya bir Intune veya EMS lisansı atanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="678de-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="678de-115">Office Yönetim Merkezi veya Azure Portal aracılığıyla lisans atamak için bu belgeleri gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="678de-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="678de-116">Sorununuzu çözmek için ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="678de-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="678de-117">Yaygın kayıt hatalarını tanılamak ve çözmek için [Intune sorun giderme portalı](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 'nı kullanın.</span><span class="sxs-lookup"><span data-stu-id="678de-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="678de-118">Daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) inceleyin.</span><span class="sxs-lookup"><span data-stu-id="678de-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="678de-119">Her biri için kayıt ve çözünürlüğe engel olan yaygın hataların listesi için [Bu belgeyi](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) inceleyin.</span><span class="sxs-lookup"><span data-stu-id="678de-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="678de-120">[Android cihazlarını Microsoft Intune 'da kaydettirme hakkında bilgi edinin](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="678de-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
