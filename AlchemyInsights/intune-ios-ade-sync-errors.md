---
title: Apple Otomatik Cihaz Kaydı eşitleme hataları
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448942"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="965de-102">Apple Otomatik Cihaz Kaydı eşitleme hataları</span><span class="sxs-lookup"><span data-stu-id="965de-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="965de-103">"Bir veya birden çok ADE/DEP Belirtecinin hata durumuna sahip olduğunu algıladık.</span><span class="sxs-lookup"><span data-stu-id="965de-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="965de-104">Etkilenen her belirteç için hata durumu çözülene kadar ADE işlevi beklendiği gibi çalışmayacak."</span><span class="sxs-lookup"><span data-stu-id="965de-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="965de-105">Bu hata çeşitli yollarla ortaya çıkar:</span><span class="sxs-lookup"><span data-stu-id="965de-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="965de-106">Cihazlar ABM/ASM'den Intune'a eşitleyene</span><span class="sxs-lookup"><span data-stu-id="965de-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="965de-107">Kayıt profili atamaları başarısız olabilir</span><span class="sxs-lookup"><span data-stu-id="965de-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="965de-108">Cihazlar ADE kaydı başarıyla tamamlanamadı</span><span class="sxs-lookup"><span data-stu-id="965de-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="965de-109">Intune konsolunda Cihazlar ve Cihazları Kaydetme > Apple kayıt > Kayıt programı belirteçleri > bildirilen eşitleme **hatasını kontrol edin.**</span><span class="sxs-lookup"><span data-stu-id="965de-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="965de-110">Eşitleme hatasının en yaygın nedenlerinden biri, geçerli belirtecin süresinin dolmasıdır.</span><span class="sxs-lookup"><span data-stu-id="965de-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="965de-111">Çoğu durumda, etkilenen belirtecin yenilenmesi sorunu çözer.</span><span class="sxs-lookup"><span data-stu-id="965de-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="965de-112">Belirteçlerin birinin veya daha fazlasının süresi dolduğunda, uygun şekilde yenilemenize yardımcı olması için aşağıdaki belgelere bakın:</span><span class="sxs-lookup"><span data-stu-id="965de-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="965de-113">Otomatik Cihaz Kaydı belirteci yenileme</span><span class="sxs-lookup"><span data-stu-id="965de-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="965de-114">Buna ek olarak, belirteç eşitleme hatalarına neden olan diğer hataların olası düzeltmelerini görmek için aşağıdaki belgeleri de bulabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="965de-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="965de-115">iOS/iPadOS ve macOS Otomatik Cihaz Kaydı Belirteçleri için ABM/ASM Eşitleme Hataları</span><span class="sxs-lookup"><span data-stu-id="965de-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="965de-116">iOS/iPadOS ve macOS Otomatik Cihaz Kaydı Belirteçleri için ABM/ASM Eşitleme Hataları</span><span class="sxs-lookup"><span data-stu-id="965de-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
