---
title: Microsoft Intune'da Android cihazlarını kaydetmeyle ilgili sorunları giderme
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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709018"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="26e54-102">Microsoft Intune'da Android cihazlarını kaydetmeyle ilgili sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="26e54-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="26e54-103">Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="26e54-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="26e54-104">Sık karşılaşılan bazı sorunlar ve çözüm adımları:</span><span class="sxs-lookup"><span data-stu-id="26e54-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="26e54-105">**Şirket Portalında Cihaz Şifreli değil hatası:** Özellikle v7.0 ile başlayan daha yeni Android sürümleri, cihazınızın tamamen şifrelenmiş olduğundan emin olmak için başlangıç geçiş kodu gerektirir.</span><span class="sxs-lookup"><span data-stu-id="26e54-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="26e54-106">Yaygın çözümler, bir başlangıç pin'ini etkinleştirmek veya cihazı tamamen şifrelemektir.</span><span class="sxs-lookup"><span data-stu-id="26e54-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="26e54-107">Daha [fazla bilgi için](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) bu belgeyi gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="26e54-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="26e54-108">**Cihazlar Intune hizmetiyle iade başarısız oluyor veya Intune yönetici konsolunda "Sağlıksız" olarak görüntüleniyor:** Bazı Samsung 4.4 ve 5.5 cihazları hizmette yer alamayyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="26e54-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="26e54-109">Bu sorunun 3 olası çözümü vardır:</span><span class="sxs-lookup"><span data-stu-id="26e54-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="26e54-110">Cihaz eşitlemeyi otomatik olarak başlatan Intune Şirket Portalı uygulamasını el ile açın.</span><span class="sxs-lookup"><span data-stu-id="26e54-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="26e54-111">Cihazı Android 6.0 veya daha yeni bir sürümüne güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="26e54-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="26e54-112">Samsung Smart Manager'ın Intune Şirket Portalı'nın yönetiminden devre dışı bırakma.</span><span class="sxs-lookup"><span data-stu-id="26e54-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="26e54-113">Bu [sorunlar ve](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) çözümle ilgili daha ayrıntılı bilgi için bu belgeyi gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="26e54-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="26e54-114">**Kullanıcı Lisans Türü Geçersiz** veya **Kullanıcı Adı Tanınmadı hatası:** Kullanıcıya Intune veya EMS lisansı atanıyor olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="26e54-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="26e54-115">Şu belgeleri gözden geçirerek lisans atabilirsiniz: Office Yönetim Merkezi veya Azure portalı.</span><span class="sxs-lookup"><span data-stu-id="26e54-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="26e54-116">Sorununuzu çözmenize yardımcı olacak ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="26e54-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="26e54-117">Yaygın [kayıt hatalarını tanılamak ve](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) çözmek için Intune Sorun Giderme Portalı'nın kullanın.</span><span class="sxs-lookup"><span data-stu-id="26e54-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="26e54-118">Daha [fazla ayrıntı için](https://docs.microsoft.com/intune/help-desk-operators) bu belgeyi gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="26e54-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="26e54-119">Her [biri için](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) kayıt ve çözüm engelleyen yaygın hataların listesi için bu belgeyi gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="26e54-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="26e54-120">[Android cihazlarını Microsoft Intune'a kaydetmeyi öğrenin.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="26e54-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
