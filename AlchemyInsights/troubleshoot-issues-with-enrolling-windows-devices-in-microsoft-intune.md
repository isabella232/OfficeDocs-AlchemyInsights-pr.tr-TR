---
title: Kaydolma Microsoft Intune aygıtlar Windows ile sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8c5e7cc502d016ad658383685523dc240dfb4dc6
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661586"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="050fc-102">Kaydolma Microsoft Intune aygıtlar Windows ile sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="050fc-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="050fc-103">Şimdi, sorunu gidermek için aşağıda listelenen kaynakları inceleyin.</span><span class="sxs-lookup"><span data-stu-id="050fc-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="050fc-104">Bazı yaygın hata iletileri ve çözümleme adımları:</span><span class="sxs-lookup"><span data-stu-id="050fc-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="050fc-p101">**Yazılımı yüklenemiyor, 0x80cf4017:** Hesap sertifikanızın süresi dolmuş. Intune yönetim konsolunda PC istemci yazılım paketini yeniden yükleyin. Daha fazla bilgi için bu belge gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="050fc-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="050fc-108">**0x801c0003 hata kodu:** Hata aşağıdaki senaryolarda ortaya çıkabilir:</span><span class="sxs-lookup"><span data-stu-id="050fc-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="050fc-p102">Daha fazla aygıtlar Aygıt üst sınırından kayıtlı kullanıcı vardır. [Bir aygıtı kaldırmak](https://docs.microsoft.com/intune/devices-wipe) veya [aygıt bu sınırı değiştirmek](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)için bu belgeleri gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="050fc-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="050fc-p103">"Kullanıcıların aygıtlar için Azure AD katılabilirsiniz" "yok" olarak ayarlanır. Tümüne ayarlayın veya seçin kullanıcılar. Daha fazla bilgi için [Bu belge](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="050fc-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="050fc-p104">Aygıt zaten başka bir kullanıcı tarafından kaydedilmiş. Bu durumda, aygıt Azure Intune konsoldan kaldırmak veya yeniden denemeden önce aygıtı el ile unenroll.</span><span class="sxs-lookup"><span data-stu-id="050fc-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="050fc-p105">Windows 10 giriş aygıtıdır. Azure Active Directory, yalnızca Windows 10 Pro, eğitim ve Kurumsal SKU'ları katılabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="050fc-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="050fc-118">Sorununuzu gidermeye yardımcı olmak için ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="050fc-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="050fc-p106">[Intune sorun giderme Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) tanılamak ve ortak kayıt hatalarını gidermek için kullanın. Daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="050fc-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="050fc-121">Bu belgeler için kayıt ve çözümler için her önlemek sık karşılaşılan hataların listesini gözden geçirin: [sorun giderme kılavuzu](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ve [sorun giderme doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="050fc-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="050fc-122">[Microsoft Intune Windows aygıtları kaydetmek öğrenin](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="050fc-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

