---
title: Kaydolma Microsoft Intune aygıtlar Windows ile sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559681"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="a4bb3-102">Kaydolma Microsoft Intune aygıtlar Windows ile sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="a4bb3-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="a4bb3-103">Şimdi, sorunu gidermek için aşağıda listelenen kaynakları inceleyin.</span><span class="sxs-lookup"><span data-stu-id="a4bb3-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="a4bb3-104">Bazı yaygın hata iletileri ve çözümleme adımları:</span><span class="sxs-lookup"><span data-stu-id="a4bb3-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="a4bb3-105">**Yazılımı yüklenemiyor, 0x80cf4017:** Hesap sertifikanızın süresi dolmuş.</span><span class="sxs-lookup"><span data-stu-id="a4bb3-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="a4bb3-106">Intune yönetim konsolunda PC istemci yazılım paketini yeniden yükleyin.</span><span class="sxs-lookup"><span data-stu-id="a4bb3-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="a4bb3-107">Daha fazla bilgi için bu belge gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="a4bb3-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="a4bb3-108">**0x801c0003 hata kodu:** Hata aşağıdaki senaryolarda ortaya çıkabilir:</span><span class="sxs-lookup"><span data-stu-id="a4bb3-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="a4bb3-109">Daha fazla aygıtlar Aygıt üst sınırından kayıtlı kullanıcı vardır.</span><span class="sxs-lookup"><span data-stu-id="a4bb3-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="a4bb3-110">[Bir aygıtı kaldırmak](https://docs.microsoft.com/intune/devices-wipe) veya [aygıt bu sınırı değiştirmek](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)için bu belgeleri gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="a4bb3-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="a4bb3-111">"Kullanıcıların aygıtlar için Azure AD katılabilirsiniz" "yok" olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="a4bb3-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="a4bb3-112">Tümüne ayarlayın veya seçin kullanıcılar.</span><span class="sxs-lookup"><span data-stu-id="a4bb3-112">Set it to all or select users.</span></span> <span data-ttu-id="a4bb3-113">Daha fazla bilgi için [Bu belge](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="a4bb3-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="a4bb3-114">Aygıt zaten başka bir kullanıcı tarafından kaydedilmiş.</span><span class="sxs-lookup"><span data-stu-id="a4bb3-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="a4bb3-115">Bu durumda, aygıt Azure Intune konsoldan kaldırmak veya yeniden denemeden önce aygıtı el ile unenroll.</span><span class="sxs-lookup"><span data-stu-id="a4bb3-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="a4bb3-116">Windows 10 giriş aygıtıdır.</span><span class="sxs-lookup"><span data-stu-id="a4bb3-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="a4bb3-117">Azure Active Directory, yalnızca Windows 10 Pro, eğitim ve Kurumsal SKU'ları katılabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a4bb3-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="a4bb3-118">Sorununuzu gidermeye yardımcı olmak için ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="a4bb3-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="a4bb3-119">[Intune sorun giderme Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) tanılamak ve ortak kayıt hatalarını gidermek için kullanın.</span><span class="sxs-lookup"><span data-stu-id="a4bb3-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="a4bb3-120">Daha fazla ayrıntı için [Bu belgeyi](https://docs.microsoft.com/intune/help-desk-operators) gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="a4bb3-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="a4bb3-121">Bu belgeler için kayıt ve çözümler için her önlemek sık karşılaşılan hataların listesini gözden geçirin: [sorun giderme kılavuzu](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ve [sorun giderme doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="a4bb3-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="a4bb3-122">[Microsoft Intune Windows aygıtları kaydetmek öğrenin](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="a4bb3-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
