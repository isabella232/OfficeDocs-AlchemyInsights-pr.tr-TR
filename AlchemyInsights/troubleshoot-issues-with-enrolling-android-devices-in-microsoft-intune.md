---
title: Microsoft Intune'da Android cihazlarını kaydetmeyle ilgili sorunları giderme
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830962"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="1b750-102">Microsoft Intune'da Android cihazlarını kaydetmeyle ilgili sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="1b750-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="1b750-103">Sorununuzu çözmek için aşağıda listelenen kaynakları gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1b750-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="1b750-104">Sık karşılaşılan bazı sorunlar ve çözüm adımları:</span><span class="sxs-lookup"><span data-stu-id="1b750-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="1b750-105">**Şirket Portalında Şifrelenmiş Değil hatası:** Özellikle v7.0 ile başlayan yeni Android sürümleri, cihazınızın tümüyle şifre olduğundan emin olmak için bir başlangıç geçiş kodu gerektirir.</span><span class="sxs-lookup"><span data-stu-id="1b750-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="1b750-106">Yaygın çözümler, bir başlangıç PIN'ini etkinleştirmek veya cihazı tam olarak şifrelemektir.</span><span class="sxs-lookup"><span data-stu-id="1b750-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="1b750-107">Daha [fazla bilgi için](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) bu belgeyi gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1b750-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="1b750-108">**Cihazlar Intune hizmetiyle iade başarısız olur veya Intune** yönetim konsolunda "Sağlıksız" olarak görüntülenir: Bazı Samsung 4.4 ve 5.5 cihazları hizmeti kontrol edeyemmektedir.</span><span class="sxs-lookup"><span data-stu-id="1b750-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="1b750-109">Bu sorunun 3 olası çözümü vardır:</span><span class="sxs-lookup"><span data-stu-id="1b750-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="1b750-110">Cihaz eşitlemeyi otomatik olarak başlatan Intune Şirket Portalı uygulamasını el ile açın.</span><span class="sxs-lookup"><span data-stu-id="1b750-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="1b750-111">Cihazı Android 6.0 veya daha yeni bir sürümüne güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="1b750-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="1b750-112">Samsung Smart Manager'ın Intune Şirket Portalı'ni yönetmesini devre dışı bırak.</span><span class="sxs-lookup"><span data-stu-id="1b750-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="1b750-113">Bu [sorunlar ve](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) çözümle ilgili daha ayrıntılı bilgi için bu belgeyi gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1b750-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="1b750-114">**Kullanıcı Lisans Türü Geçersiz** **veya Kullanıcı Adı Tanınmadı hatası:** Kullanıcıya Intune veya EMS lisansı atanıyor olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="1b750-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="1b750-115">Lisans atamak için şu belgeleri gözden geçirebilirsiniz: Office Yönetim Merkezi veya Azure portalı.</span><span class="sxs-lookup"><span data-stu-id="1b750-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="1b750-116">Sorununuzu çözmenize yardımcı olacak ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="1b750-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="1b750-117">Yaygın kayıt sorunlarını tanılamak ve gidermek için [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) Sorun Giderme Portalı'nın kullanın.</span><span class="sxs-lookup"><span data-stu-id="1b750-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="1b750-118">Daha [fazla ayrıntı için](https://docs.microsoft.com/intune/help-desk-operators) bu belgeyi gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1b750-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="1b750-119">Kayıt [ve çözümlerini](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) engelleyen yaygın hataların listesi için bu belgeyi gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1b750-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="1b750-120">[Android cihazları Microsoft Intune'a nasıl kaydeden öğrenin.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="1b750-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
