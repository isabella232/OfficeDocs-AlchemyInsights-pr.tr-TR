---
title: Microsoft Intune 'da iOS cihazlarını kaydetme sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669268"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="bf25b-102">Microsoft Intune 'da iOS cihazlarını kaydetme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="bf25b-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="bf25b-103">Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="bf25b-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="bf25b-104">Bazı yaygın hata iletileri ve çözüm adımları:</span><span class="sxs-lookup"><span data-stu-id="bf25b-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="bf25b-105">**Cihaz Cap 'e ulaşıldı** Kullanıcının cihaz sınırından daha fazla kayıtlı cihazı var.</span><span class="sxs-lookup"><span data-stu-id="bf25b-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="bf25b-106">[Cihazı kaldırmak](https://docs.microsoft.com/intune/devices-wipe) veya [cihaz sınırını değiştirmek](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)için bu belgeleri gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="bf25b-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="bf25b-107">**Bu hizmet desteklenmiyor. Kayıt Ilkesi yok:** Apple anında bildirim hizmeti (APNs) yapılandırılmalı veya yenilenmelidir.</span><span class="sxs-lookup"><span data-stu-id="bf25b-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="bf25b-108">Bunun nasıl yapıldığını açıklayan yönergeler için [Bu belgeyi](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) inceleyin.</span><span class="sxs-lookup"><span data-stu-id="bf25b-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="bf25b-109">**Kullanıcı Lisans türü geçersiz veya Kullanıcı adı tanınmadı:** Kullanıcıya bir Intune veya EMS lisansı atanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="bf25b-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="bf25b-110">[Office Yönetim Merkezi](https://docs.microsoft.com/intune/licenses-assign) veya [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups)aracılığıyla lisans atamak için bu belgeleri gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="bf25b-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="bf25b-111">Sorununuzu çözmek için ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="bf25b-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="bf25b-112">Yaygın kayıt hatalarını tanılamak ve çözmek için [Intune sorun giderme portalı](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 'nı kullanın.</span><span class="sxs-lookup"><span data-stu-id="bf25b-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="bf25b-113">Daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) inceleyin.</span><span class="sxs-lookup"><span data-stu-id="bf25b-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="bf25b-114">Her biri için kayıt ve çözünürlüğe engel olan yaygın hataların listesi için bu belgeleri gözden geçirin: [sorun giderme kılavuzu](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ve [belge sorunlarını giderme](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="bf25b-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="bf25b-115">[Microsoft Intune 'Da iOS cihazlarını kaydettirme hakkında bilgi edinin](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="bf25b-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

