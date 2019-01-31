---
title: Microsoft Intune IOS aygıtları kaydolma sorunları giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: cd1afc83fe98f363aee4c3324a634c200cd08947
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658459"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="843d2-102">Microsoft Intune IOS aygıtları kaydolma sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="843d2-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="843d2-103">Şimdi, sorunu gidermek için aşağıda listelenen kaynakları inceleyin.</span><span class="sxs-lookup"><span data-stu-id="843d2-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="843d2-104">Bazı yaygın hata iletileri ve çözümleme adımları:</span><span class="sxs-lookup"><span data-stu-id="843d2-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="843d2-p101">**Aygıt Cap ulaştı** Daha fazla aygıtlar Aygıt üst sınırından kayıtlı kullanıcı vardır. [Bir aygıtı kaldırmak](https://docs.microsoft.com/intune/devices-wipe) veya [aygıt bu sınırı değiştirmek](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)için bu belgeleri gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="843d2-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="843d2-p102">**Bu hizmeti desteklenmiyor. Hiçbir kayıt ilkesi:** yapılandırılmış veya yenilenmiş elma itme bildirim hizmeti (APNS) gerekir. Bunu yapmak yönergeler için [Bu belgeyi](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="843d2-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="843d2-p103">**Kullanıcı lisans türü geçersiz veya tanınmayan kullanıcı adı:** Kullanıcı bir Intune veya EMS lisans atanması gerekir. Bir lisans aracılığıyla atamak için bu belgeleri gözden geçirin: [Office Yönetim Merkezi](https://docs.microsoft.com/intune/licenses-assign) veya [Azure portalı](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="843d2-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="843d2-111">Sorununuzu gidermeye yardımcı olmak için ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="843d2-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="843d2-p104">[Intune sorun giderme Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) tanılamak ve ortak kayıt hatalarını gidermek için kullanın. Daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="843d2-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="843d2-114">Bu belgeler için kayıt ve çözümler için her önlemek sık karşılaşılan hataların listesini gözden geçirin: [sorun giderme kılavuzu](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ve [sorun giderme doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="843d2-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="843d2-115">[Microsoft Intune IOS aygıtları kaydetmek öğrenin](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="843d2-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

