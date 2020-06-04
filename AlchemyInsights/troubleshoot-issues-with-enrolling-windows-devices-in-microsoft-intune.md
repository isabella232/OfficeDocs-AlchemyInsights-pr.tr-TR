---
title: Windows aygıtlarını Microsoft Intune'a kaydetme yle ilgili sorun giderme sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665852"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="408c5-102">Windows aygıtlarını Microsoft Intune'a kaydetme yle ilgili sorun giderme sorunları</span><span class="sxs-lookup"><span data-stu-id="408c5-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="408c5-103">Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="408c5-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="408c5-104">Bazı yaygın hata iletileri ve çözüm adımları:</span><span class="sxs-lookup"><span data-stu-id="408c5-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="408c5-105">**Yazılım, 0x80cf4017 yüklenemez:** Hesap sertifikanızın süresi doldu.</span><span class="sxs-lookup"><span data-stu-id="408c5-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="408c5-106">PC Client yazılım paketini Intune Admin Konsoluna yeniden indirin.</span><span class="sxs-lookup"><span data-stu-id="408c5-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="408c5-107">Daha fazla bilgi için bu belgeleri gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="408c5-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="408c5-108">**Hata kodu 0x801c0003:** Hata aşağıdaki senaryolarda oluşabilir:</span><span class="sxs-lookup"><span data-stu-id="408c5-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="408c5-109">Kullanıcı, aygıt sınırından daha fazla aygıt alabilenir.</span><span class="sxs-lookup"><span data-stu-id="408c5-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="408c5-110">[Aygıtı kaldırmak](https://docs.microsoft.com/intune/devices-wipe) veya aygıt [sınırını değiştirmek](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)için bu belgeleri gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="408c5-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="408c5-111">"Kullanıcılar aygıtları Azure AD'ye katılabilir" olarak ayarlanır".</span><span class="sxs-lookup"><span data-stu-id="408c5-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="408c5-112">Tüm ünü veya belirli kullanıcılara ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="408c5-112">Set it to all or select users.</span></span> <span data-ttu-id="408c5-113">Daha fazla bilgi için [bu belgeleri](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="408c5-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="408c5-114">Aygıt zaten başka bir kullanıcı tarafından kaydedilen.</span><span class="sxs-lookup"><span data-stu-id="408c5-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="408c5-115">Bu durumda, yeniden denemeden önce aygıtı Azure Intune konsolundan çıkarın veya aygıtı el ile kaldırın.</span><span class="sxs-lookup"><span data-stu-id="408c5-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="408c5-116">Cihaz Windows 10 Home'dur.</span><span class="sxs-lookup"><span data-stu-id="408c5-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="408c5-117">Azure Active Directory'ye yalnızca Windows 10 Pro, Eğitim ve Kurumsal SK'ler katılabilir.</span><span class="sxs-lookup"><span data-stu-id="408c5-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="408c5-118">Sorununuzu çözmeye yardımcı olacak ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="408c5-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="408c5-119">Sık karşılaşılan kayıt hatalarını tanılamak ve gidermek için [Intune Sorun Giderme Portalı'nı](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) kullanın.</span><span class="sxs-lookup"><span data-stu-id="408c5-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="408c5-120">Daha fazla ayrıntı için [bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="408c5-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="408c5-121">Bu belgeleri, her birine kaydolmasını ve çözümlerini engelleyen yaygın hataların bir listesi için gözden geçirin: [Sorun Giderme kılavuzu](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ve [Sorun Giderme dokümanı.](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="408c5-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="408c5-122">[Windows aygıtlarını Microsoft Intune'a nasıl kaydedebilirsiniz öğrenin.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="408c5-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
