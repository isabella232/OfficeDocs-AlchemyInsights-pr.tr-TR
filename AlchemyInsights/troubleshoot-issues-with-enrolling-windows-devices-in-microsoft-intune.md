---
title: Windows cihazlarını Microsoft Intune'a kaydetmeyle ilgili sorunları giderme
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
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708910"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="7164a-102">Windows cihazlarını Microsoft Intune'a kaydetmeyle ilgili sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="7164a-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="7164a-103">Sorununuzu şimdi çözmek için aşağıda listelenen kaynakları gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7164a-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="7164a-104">Sık karşılaşılan bazı hata iletileri ve çözüm adımları:</span><span class="sxs-lookup"><span data-stu-id="7164a-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="7164a-105">**Yazılım yük olamaz, 0x80cf4017:** Hesap sertifikanın süresi doldu.</span><span class="sxs-lookup"><span data-stu-id="7164a-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="7164a-106">Intune Yönetim Konsolu'nu kullanarak BILGISAYAR İstemcisi yazılım paketini yeniden indirin.</span><span class="sxs-lookup"><span data-stu-id="7164a-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="7164a-107">Daha fazla bilgi için bu belgeleri gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7164a-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="7164a-108">**Hata kodu 0x801c0003:** Hata aşağıdaki senaryolarda oluşabilir:</span><span class="sxs-lookup"><span data-stu-id="7164a-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="7164a-109">Kullanıcının cihaz sınırının üzerinde kayıtlı cihazı var.</span><span class="sxs-lookup"><span data-stu-id="7164a-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="7164a-110">Bir cihazı kaldırmak veya [cihaz sınırını değiştirmek](https://docs.microsoft.com/intune/devices-wipe) için bu belgeleri gözden [geçirebilirsiniz.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="7164a-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="7164a-111">"Kullanıcılar cihazları Azure AD'ye katılabilir" olarak "yok" olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="7164a-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="7164a-112">Bunu tüm kullanıcılara veya belirli kullanıcılara ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="7164a-112">Set it to all or select users.</span></span> <span data-ttu-id="7164a-113">Daha [fazla bilgi için bu](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) belgeleri gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7164a-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="7164a-114">Cihaz zaten başka bir kullanıcı tarafından kayıtlı.</span><span class="sxs-lookup"><span data-stu-id="7164a-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="7164a-115">Böyle bir durumda, cihazı Azure Intune konsolundan kaldırın veya yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="7164a-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="7164a-116">Cihaz Windows 10 Home'tır.</span><span class="sxs-lookup"><span data-stu-id="7164a-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="7164a-117">Azure Active Directory'ye yalnızca Windows 10 Pro, Eğitim ve Kurumsal SKUs katılabilir.</span><span class="sxs-lookup"><span data-stu-id="7164a-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="7164a-118">Sorununuzu çözmenize yardımcı olacak ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="7164a-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="7164a-119">Yaygın [kayıt hatalarını tanılamak ve](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) çözmek için Intune Sorun Giderme Portalı'nın kullanın.</span><span class="sxs-lookup"><span data-stu-id="7164a-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="7164a-120">Daha [fazla ayrıntı için](https://docs.microsoft.com/intune/help-desk-operators) bu belgeyi gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7164a-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="7164a-121">Her biri için kayıt ve çözümleri engelleyen yaygın hataların listesi için bu belgeleri gözden geçirme: Sorun giderme [kılavuzu ve](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) Sorun [giderme belgesi.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="7164a-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="7164a-122">[Windows cihazlarını Microsoft Intune'a kaydetmeyi öğrenin.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="7164a-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
