---
title: Microsoft Intune Android aygıtlar kaydolma sorunları giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655903"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="6c32a-102">Microsoft Intune Android aygıtlar kaydolma sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="6c32a-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="6c32a-103">Şimdi, sorunu gidermek için aşağıda listelenen kaynakları inceleyin.</span><span class="sxs-lookup"><span data-stu-id="6c32a-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="6c32a-104">Bazı sık karşılaşılan sorunlar ve çözüm adımları:</span><span class="sxs-lookup"><span data-stu-id="6c32a-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="6c32a-p101">**Aygıt şifreli şirket Portal hatası:** Android, özellikle v7.0 ile başlayan yeni sürümleri, aygıt tam olarak şifrelendiğinden emin olmak için bir başlangıç parolası gerektirir. Başlangıç PIN'i etkinleştirmek veya aygıt tam olarak şifrelemek için ortak çözümler şunlardır. Daha fazla bilgi için [Bu belgeyi](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="6c32a-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="6c32a-p102">**Aygıtları başarısız Intune hizmeti ile denetlemek veya Intune yönetim konsolunda "Sağlıksız" görüntülemek:** Bazı Samsung 4.4 ve 5.5 aygıtları hizmette oturum denetimi yapamayabilirsiniz. Bu sorundan 3 olası çözümler şunlardır:</span><span class="sxs-lookup"><span data-stu-id="6c32a-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="6c32a-110">Otomatik olarak bir aygıt eşitleme başlatacağı Intune şirket Portal uygulamayı el ile açın.</span><span class="sxs-lookup"><span data-stu-id="6c32a-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="6c32a-111">Android 6.0 veya daha fazla aygıt güncelleştirin.</span><span class="sxs-lookup"><span data-stu-id="6c32a-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="6c32a-p103">Samsung akıllı Yöneticisi dan Intune şirket Portal Yönetimi devre dışı bırakın. Bu sorunlar ve çözümleri hakkında daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="6c32a-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="6c32a-p104">**Kullanıcı lisans türü geçersiz** veya **kullanıcı adı tanınmadı hatası:** kullanıcı Intune veya EMS bir lisans atanması gerekir. Bir lisans aracılığıyla atamak için bu belgeleri gözden geçirin: Office Yönetim Merkezi veya Azure portal.</span><span class="sxs-lookup"><span data-stu-id="6c32a-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="6c32a-116">Sorununuzu gidermeye yardımcı olmak için ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="6c32a-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="6c32a-p105">[Intune sorun giderme Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) tanılamak ve ortak kayıt hatalarını gidermek için kullanın. Daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="6c32a-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="6c32a-119">[Bu belge](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) için kayıt ve çözümler için her önlemek sık karşılaşılan hataların listesini gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="6c32a-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="6c32a-120">[Microsoft Intune Android aygıtlar kaydetmeyi öğrenin](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="6c32a-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

