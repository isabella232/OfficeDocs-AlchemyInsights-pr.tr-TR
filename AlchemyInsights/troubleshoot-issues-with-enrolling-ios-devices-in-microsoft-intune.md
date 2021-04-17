---
title: Microsoft Intune'da iOS cihazlarını kaydetmeyle ilgili sorunları giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823483"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="4d1d7-102">Microsoft Intune'da iOS cihazlarını kaydetmeyle ilgili sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="4d1d7-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="4d1d7-103">Sorununuzu çözmek için aşağıda listelenen kaynakları gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4d1d7-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="4d1d7-104">Sık karşılaşılan bazı hata iletileri ve çözüm adımları:</span><span class="sxs-lookup"><span data-stu-id="4d1d7-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="4d1d7-105">**Cihaz Başlığına Ulaşıldı** Kullanıcının cihaz sınırının üzerinde kayıtlı cihazı var.</span><span class="sxs-lookup"><span data-stu-id="4d1d7-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="4d1d7-106">Cihazı kaldırmak veya [cihaz sınırını değiştirmek için](https://docs.microsoft.com/intune/devices-wipe) bu belgeleri gözden [geçirebilirsiniz.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="4d1d7-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="4d1d7-107">**Bu Hizmet desteklenmiyor. Kayıt İlkesi Yok:** Apple Anında Bildirim Hizmeti (APNS) yapılandırıldığında veya yenilenmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="4d1d7-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="4d1d7-108">Bunu [nasıl yapmaya](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) yönelik yönergeler için bu belgeyi gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4d1d7-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="4d1d7-109">**Kullanıcı Lisans Türü Geçersiz veya Kullanıcı Adı Tanınmıyor:** Kullanıcıya Intune veya EMS lisansı atanıyor olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="4d1d7-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="4d1d7-110">Lisans atamak için şu belgeleri gözden geçirebilirsiniz: [Office Yönetim Merkezi](https://docs.microsoft.com/intune/licenses-assign) veya Azure [portalı.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="4d1d7-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="4d1d7-111">Sorununuzu çözmenize yardımcı olacak ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="4d1d7-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="4d1d7-112">Yaygın kayıt sorunlarını tanılamak ve gidermek için [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) Sorun Giderme Portalı'nın kullanın.</span><span class="sxs-lookup"><span data-stu-id="4d1d7-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="4d1d7-113">Daha [fazla ayrıntı için](https://docs.microsoft.com/intune/help-desk-operators) bu belgeyi gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4d1d7-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="4d1d7-114">Kayıt ve çözümleri engelleyen yaygın hataların listesi için bu belgeleri gözden geçirebilirsiniz: Sorun giderme [kılavuzu](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ve [Sorun giderme belgesi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="4d1d7-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="4d1d7-115">[Microsoft Intune'da iOS cihazlarını kaydetmeyi öğrenin.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="4d1d7-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

