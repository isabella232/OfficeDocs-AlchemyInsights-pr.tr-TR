---
title: Microsoft Intune'da Windows cihazlarını kaydetmeyle ilgili sorunları giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808991"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="4ef5e-102">Microsoft Intune'da Windows cihazlarını kaydetmeyle ilgili sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="4ef5e-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="4ef5e-103">Sorununuzu çözmek için aşağıda listelenen kaynakları gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4ef5e-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="4ef5e-104">Sık karşılaşılan bazı hata iletileri ve çözüm adımları:</span><span class="sxs-lookup"><span data-stu-id="4ef5e-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="4ef5e-105">**Yazılım yük olamaz, 0x80cf4017:** Hesap sertifikanın süresi doldu.</span><span class="sxs-lookup"><span data-stu-id="4ef5e-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="4ef5e-106">Intune Yönetim Konsolu'nu kullanarak BILGISAYAR İstemcisi yazılım paketini yeniden indirin.</span><span class="sxs-lookup"><span data-stu-id="4ef5e-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="4ef5e-107">Daha fazla bilgi için bu belgeleri gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4ef5e-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="4ef5e-108">**Hata kodu 0x801c0003:** Hata aşağıdaki senaryolarda oluşabilir:</span><span class="sxs-lookup"><span data-stu-id="4ef5e-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="4ef5e-109">Kullanıcının cihaz sınırının üzerinde kayıtlı cihazı var.</span><span class="sxs-lookup"><span data-stu-id="4ef5e-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="4ef5e-110">Cihazı kaldırmak veya [cihaz sınırını değiştirmek için](https://docs.microsoft.com/intune/devices-wipe) bu belgeleri gözden [geçirebilirsiniz.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="4ef5e-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="4ef5e-111">"Kullanıcılar Azure AD'ye cihazlara katılabilir" olarak "yok" ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="4ef5e-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="4ef5e-112">Tüm kullanıcılara ayarlayın veya kullanıcıları seçin.</span><span class="sxs-lookup"><span data-stu-id="4ef5e-112">Set it to all or select users.</span></span> <span data-ttu-id="4ef5e-113">Daha [fazla bilgi için bu](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) belgeleri gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4ef5e-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="4ef5e-114">Cihaz başka bir kullanıcı tarafından zaten kayıtlı.</span><span class="sxs-lookup"><span data-stu-id="4ef5e-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="4ef5e-115">Böyle bir durumda, yeniden çalışmadan önce cihazı Azure Intune konsolundan kaldırın veya el ile kaydı kaldırın.</span><span class="sxs-lookup"><span data-stu-id="4ef5e-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="4ef5e-116">Cihaz, Windows 10 Home'dır.</span><span class="sxs-lookup"><span data-stu-id="4ef5e-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="4ef5e-117">Azure Active Directory'ye yalnızca Windows 10 Pro, Eğitim ve Kurumsal SKUs katılabilir.</span><span class="sxs-lookup"><span data-stu-id="4ef5e-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="4ef5e-118">Sorununuzu çözmenize yardımcı olacak ek kaynaklar:</span><span class="sxs-lookup"><span data-stu-id="4ef5e-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="4ef5e-119">Yaygın kayıt sorunlarını tanılamak ve gidermek için [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) Sorun Giderme Portalı'nın kullanın.</span><span class="sxs-lookup"><span data-stu-id="4ef5e-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="4ef5e-120">Daha [fazla ayrıntı için](https://docs.microsoft.com/intune/help-desk-operators) bu belgeyi gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="4ef5e-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="4ef5e-121">Kayıt ve çözümleri engelleyen yaygın hataların listesi için bu belgeleri gözden geçirebilirsiniz: Sorun giderme [kılavuzu](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ve [Sorun giderme belgesi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="4ef5e-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="4ef5e-122">[Windows cihazlarını Microsoft Intune'a nasıl kaydedtiklerini öğrenin.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="4ef5e-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
