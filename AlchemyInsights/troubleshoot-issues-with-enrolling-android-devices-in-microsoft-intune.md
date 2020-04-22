---
title: Android cihazlarımicrosoft Intune'a kaydetme yle ilgili sorun giderme sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759640"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="783a0-102">Android cihazlarımicrosoft Intune'a kaydetme yle ilgili sorun giderme sorunları</span><span class="sxs-lookup"><span data-stu-id="783a0-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="783a0-103">Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="783a0-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="783a0-104">Bazı sık karşılaşılan sorunlar ve çözüm adımları:</span><span class="sxs-lookup"><span data-stu-id="783a0-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="783a0-105">**Şirket Portalında Şifrelenmemiş Aygıt Hatası:** Android'in özellikle v7.0 ile başlayan yeni sürümleri, cihazınızın tamamen şifrelenmiş olduğundan emin olmak için bir başlangıç şifresi gerektirir.</span><span class="sxs-lookup"><span data-stu-id="783a0-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="783a0-106">Ortak çözümler bir başlangıç pin etkinleştirmek veya tamamen aygıtı şifrelemek içinvardır.</span><span class="sxs-lookup"><span data-stu-id="783a0-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="783a0-107">Daha fazla bilgi için [bu belgeyi](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="783a0-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="783a0-108">**Aygıtlar Intune hizmetiyle check-in yapmayı veya Intune yönetici konsolunda "Sağlıksız" olarak görüntülenememektedir:** Bazı Samsung 4.4 ve 5.5 cihazları hizmete giriş olmayabilir.</span><span class="sxs-lookup"><span data-stu-id="783a0-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="783a0-109">Bu sorunun 3 olası çözümü vardır:</span><span class="sxs-lookup"><span data-stu-id="783a0-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="783a0-110">Bir aygıt senkronizasyonuna otomatik olarak başlayacak olan Intune Company Portal uygulamasını el ile açın.</span><span class="sxs-lookup"><span data-stu-id="783a0-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="783a0-111">Cihazı Android 6.0 veya üzeri olarak güncelleyin.</span><span class="sxs-lookup"><span data-stu-id="783a0-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="783a0-112">Samsung Smart Manager'ı Intune Company Portalını yönetmekten devre dışı edin.</span><span class="sxs-lookup"><span data-stu-id="783a0-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="783a0-113">Bu sorunlar ve çözümler hakkında daha fazla bilgi için [bu belgeyi](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="783a0-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="783a0-114">**Kullanıcı Lisans Türü Geçersiz** veya **Kullanıcı Adı Tanınmayan hata:** Kullanıcıya bir Intune veya EMS lisansı atanması gerekir.</span><span class="sxs-lookup"><span data-stu-id="783a0-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="783a0-115">Aşağıdakiler üzerinden lisans atamak için bu belgeleri gözden geçirin: Office Yönetici Merkezi veya Azure portalı.</span><span class="sxs-lookup"><span data-stu-id="783a0-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="783a0-116">Sorununuzu çözmeye yardımcı olacak ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="783a0-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="783a0-117">Sık karşılaşılan kayıt hatalarını tanılamak ve gidermek için [Intune Sorun Giderme Portalı'nı](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) kullanın.</span><span class="sxs-lookup"><span data-stu-id="783a0-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="783a0-118">Daha fazla ayrıntı için [bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="783a0-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="783a0-119">Her biri için kayıt ve çözümleri engelleyen yaygın hataların bir listesi için [bu belgeyi](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="783a0-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="783a0-120">[Android aygıtları Microsoft Intune'a nasıl kaydedebilirsiniz öğrenin.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="783a0-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
