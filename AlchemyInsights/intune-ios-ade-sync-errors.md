---
title: Apple otomatik cihaz kaydı Eşitleme hataları
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714972"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="8f007-102">Apple otomatik cihaz kaydı Eşitleme hataları</span><span class="sxs-lookup"><span data-stu-id="8f007-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="8f007-103">"Hata durumundaki bir veya birden çok ADE/DEP belirteçlerinin olduğunu algıladık.</span><span class="sxs-lookup"><span data-stu-id="8f007-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="8f007-104">Tüm etkilenen belirteçteki hata durumu çözümleninceye kadar, ADE işlevi aynı ".</span><span class="sxs-lookup"><span data-stu-id="8f007-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="8f007-105">Bu hata çeşitli yollarla bildirim alabilir:</span><span class="sxs-lookup"><span data-stu-id="8f007-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="8f007-106">Cihazlar ABR 'den Intune 'a eşitlenmeyebilir</span><span class="sxs-lookup"><span data-stu-id="8f007-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="8f007-107">Kayıt profili atamaları başarısız olabilir</span><span class="sxs-lookup"><span data-stu-id="8f007-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="8f007-108">Cihazlar ADE kaydı başarıyla tamamlayamıyor</span><span class="sxs-lookup"><span data-stu-id="8f007-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="8f007-109">Intune konsolunda bildirilen eşitleme hatasını denetleyin **> cihazlar > Apple kayıt > kayıt programı belirteçlerini** ve olası düzeltmeye bakmak için aşağıdaki belgeleri inceleyin:</span><span class="sxs-lookup"><span data-stu-id="8f007-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="8f007-110">İOS/ıpados ve macOS otomatik cihaz kayıt belirteçlerinde ABM/ASM Eşitleme hataları</span><span class="sxs-lookup"><span data-stu-id="8f007-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
