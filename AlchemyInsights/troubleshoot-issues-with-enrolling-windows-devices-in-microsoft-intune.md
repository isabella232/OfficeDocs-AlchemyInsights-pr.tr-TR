---
title: Microsoft Intune 'da Windows cihazlarını kaydetme sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658898"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="2ab82-102">Microsoft Intune 'da Windows cihazlarını kaydetme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="2ab82-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="2ab82-103">Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="2ab82-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="2ab82-104">Bazı yaygın hata iletileri ve çözüm adımları:</span><span class="sxs-lookup"><span data-stu-id="2ab82-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="2ab82-105">**Yazılım yüklenemiyor, 0x80cf4017:** Hesap sertifikanızın süresi doldu.</span><span class="sxs-lookup"><span data-stu-id="2ab82-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="2ab82-106">Intune yönetim konsolundaki PC Istemcisi yazılımı paketini yeniden indirin.</span><span class="sxs-lookup"><span data-stu-id="2ab82-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="2ab82-107">Daha fazla bilgi için bu belgeyi inceleyin.</span><span class="sxs-lookup"><span data-stu-id="2ab82-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="2ab82-108">**Hata kodu 0x801c0003:** Hata aşağıdaki senaryolarda oluşabilir:</span><span class="sxs-lookup"><span data-stu-id="2ab82-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="2ab82-109">Kullanıcının cihaz sınırından daha fazla kayıtlı cihazı var.</span><span class="sxs-lookup"><span data-stu-id="2ab82-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="2ab82-110">[Cihazı kaldırmak](https://docs.microsoft.com/intune/devices-wipe) veya [cihaz sınırını değiştirmek](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)için bu belgeleri gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="2ab82-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="2ab82-111">"Kullanıcılar cihazları Azure AD 'ye katılabilir" "yok" olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="2ab82-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="2ab82-112">Tümünü ayarlayın veya kullanıcıları seçin.</span><span class="sxs-lookup"><span data-stu-id="2ab82-112">Set it to all or select users.</span></span> <span data-ttu-id="2ab82-113">Daha fazla bilgi için [Bu belgeyi](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) inceleyin.</span><span class="sxs-lookup"><span data-stu-id="2ab82-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="2ab82-114">Cihaz zaten başka bir kullanıcı tarafından kaydedilmiş.</span><span class="sxs-lookup"><span data-stu-id="2ab82-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="2ab82-115">Bu durumda, cihazı Azure Intune konsolundan kaldırın veya yeniden denemeden önce cihazı el ile kaldırın.</span><span class="sxs-lookup"><span data-stu-id="2ab82-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="2ab82-116">Cihaz Windows 10 ev.</span><span class="sxs-lookup"><span data-stu-id="2ab82-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="2ab82-117">Yalnızca Windows 10 Pro, eğitim ve kurumsal SKU 'Lar Azure Active Directory 'ye katılabilir.</span><span class="sxs-lookup"><span data-stu-id="2ab82-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="2ab82-118">Sorununuzu çözmek için ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="2ab82-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="2ab82-119">Yaygın kayıt hatalarını tanılamak ve çözmek için [Intune sorun giderme portalı](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 'nı kullanın.</span><span class="sxs-lookup"><span data-stu-id="2ab82-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="2ab82-120">Daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) inceleyin.</span><span class="sxs-lookup"><span data-stu-id="2ab82-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="2ab82-121">Her biri için kayıt ve çözünürlüğe engel olan yaygın hataların listesi için bu belgeleri gözden geçirin: [sorun giderme kılavuzu](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ve [belge sorunlarını giderme](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="2ab82-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="2ab82-122">[Microsoft Intune 'Da Windows cihazlarını kaydettirme hakkında bilgi edinin](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="2ab82-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
