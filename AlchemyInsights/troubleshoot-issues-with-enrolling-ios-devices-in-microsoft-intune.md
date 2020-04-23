---
title: iOS aygıtlarını Microsoft Intune'a kaydetme yle ilgili sorun giderme sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736178"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="b3f98-102">iOS aygıtlarını Microsoft Intune'a kaydetme yle ilgili sorun giderme sorunları</span><span class="sxs-lookup"><span data-stu-id="b3f98-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="b3f98-103">Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="b3f98-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="b3f98-104">Bazı yaygın hata iletileri ve çözüm adımları:</span><span class="sxs-lookup"><span data-stu-id="b3f98-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="b3f98-105">**Cihaz Kapağına Ulaşıldı** Kullanıcı, aygıt sınırından daha fazla aygıt alabilenir.</span><span class="sxs-lookup"><span data-stu-id="b3f98-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="b3f98-106">[Aygıtı kaldırmak](https://docs.microsoft.com/intune/devices-wipe) veya aygıt [sınırını değiştirmek](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)için bu belgeleri gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="b3f98-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="b3f98-107">**Bu Hizmet desteklenmez. Kayıt Politikası Yok:** Apple Push Bildirim Hizmeti'nin (APNS) yapılandırılması veya yenilenmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="b3f98-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="b3f98-108">Bunun nasıl yapılacağını anlatan talimatlar için [bu belgeyi](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="b3f98-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="b3f98-109">**Kullanıcı Lisans Türü Geçersiz veya Kullanıcı Adı Tanınmadı:** Kullanıcıya bir Intune veya EMS lisansı atanması gerekir.</span><span class="sxs-lookup"><span data-stu-id="b3f98-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="b3f98-110">Lisans atamak için bu belgeleri gözden [geçirin: Office Yönetici Merkezi](https://docs.microsoft.com/intune/licenses-assign) veya [Azure portalı.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="b3f98-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="b3f98-111">Sorununuzu çözmeye yardımcı olacak ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="b3f98-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="b3f98-112">Sık karşılaşılan kayıt hatalarını tanılamak ve gidermek için [Intune Sorun Giderme Portalı'nı](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) kullanın.</span><span class="sxs-lookup"><span data-stu-id="b3f98-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b3f98-113">Daha fazla ayrıntı için [bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="b3f98-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="b3f98-114">Bu belgeleri, her birine kaydolmasını ve çözümlerini engelleyen yaygın hataların bir listesi için gözden geçirin: [Sorun Giderme kılavuzu](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ve [Sorun Giderme dokümanı.](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="b3f98-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="b3f98-115">[iOS aygıtlarını Microsoft Intune'a nasıl kaydedebilirsiniz öğrenin.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="b3f98-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

