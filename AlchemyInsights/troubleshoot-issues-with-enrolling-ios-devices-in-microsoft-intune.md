---
title: Microsoft Intune'da iOS cihazlarını kaydetmeyle ilgili sorunları giderme
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
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708982"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="b3c76-102">Microsoft Intune'da iOS cihazlarını kaydetmeyle ilgili sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="b3c76-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="b3c76-103">Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b3c76-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="b3c76-104">Sık karşılaşılan bazı hata iletileri ve çözüm adımları:</span><span class="sxs-lookup"><span data-stu-id="b3c76-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="b3c76-105">**Cihaz Başlığına Ulaşıldı** Kullanıcının cihaz sınırının üzerinde kayıtlı cihazı var.</span><span class="sxs-lookup"><span data-stu-id="b3c76-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="b3c76-106">Bir cihazı kaldırmak veya [cihaz sınırını değiştirmek](https://docs.microsoft.com/intune/devices-wipe) için bu belgeleri gözden [geçirebilirsiniz.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="b3c76-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="b3c76-107">**Bu Hizmet desteklenmiyor. Kayıt İlkesi Yok:** Apple Anında Bildirim Hizmeti'nin (APNS) yapılandırılması veya yenilenmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="b3c76-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="b3c76-108">Bunu [nasıl yapacağıma](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) ilişkin yönergeler için bu belgeyi gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b3c76-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="b3c76-109">**Kullanıcı Lisans Türü Geçersiz veya Kullanıcı Adı Tanınmıyor:** Kullanıcıya Intune veya EMS lisansı atanıyor olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="b3c76-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="b3c76-110">Şu belgeleri gözden geçirerek lisans atabilirsiniz: [Office Yönetim Merkezi veya](https://docs.microsoft.com/intune/licenses-assign) Azure [portalı.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="b3c76-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="b3c76-111">Sorununuzu çözmenize yardımcı olacak ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="b3c76-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="b3c76-112">Yaygın [kayıt hatalarını tanılamak ve](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) çözmek için Intune Sorun Giderme Portalı'nın kullanın.</span><span class="sxs-lookup"><span data-stu-id="b3c76-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b3c76-113">Daha [fazla ayrıntı için](https://docs.microsoft.com/intune/help-desk-operators) bu belgeyi gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b3c76-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="b3c76-114">Her biri için kayıt ve çözümleri engelleyen yaygın hataların listesi için bu belgeleri gözden geçirme: Sorun giderme [kılavuzu ve](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) Sorun [giderme belgesi.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="b3c76-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="b3c76-115">[iOS cihazlarını Microsoft Intune'a kaydetmeyi öğrenin.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="b3c76-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

