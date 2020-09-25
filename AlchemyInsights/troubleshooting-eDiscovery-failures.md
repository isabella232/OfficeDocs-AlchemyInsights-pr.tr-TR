---
title: 1490-sorun giderme-eBulma-hatalar
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277822"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="28820-102">Içerik arama hatalarını giderme</span><span class="sxs-lookup"><span data-stu-id="28820-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="28820-103">Arama sonuçlarını dışarı aktardığınızda Içerik aramayla ilgili sorun yaşıyor veya hata alıyor mu?</span><span class="sxs-lookup"><span data-stu-id="28820-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="28820-104">Örneğin, aramaları çalıştırırken aşağıdakileri mi alıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="28820-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="28820-105">CS008 veya CS012 hataları</span><span class="sxs-lookup"><span data-stu-id="28820-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="28820-106">Sunucu meşgul/zamanaşımı hataları</span><span class="sxs-lookup"><span data-stu-id="28820-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="28820-107">Uygulama hatası oluştu</span><span class="sxs-lookup"><span data-stu-id="28820-107">Application error occurred</span></span>

<span data-ttu-id="28820-108">Veya sonuçları çok sayıda posta kutusu (100.000 posta kutusu üzerinden) ararken veya verirken dışarı aktarma hatalarını mı alıyorsunuz?</span><span class="sxs-lookup"><span data-stu-id="28820-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="28820-109">Bu hata türleri için başarısız olan içerik konumlarını aramayı yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="28820-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="28820-110">Daha fazla bilgi için  [Bu makaleye](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) bakın.</span><span class="sxs-lookup"><span data-stu-id="28820-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="28820-111">100K posta kutularını dışarı aktarıyorsanız, dışarı aktarma sonuçlarını indirmek için aşağıdaki PowerShell 'i kullanmanız gerekir:  [100 ' den fazla posta kutusu 'ndan sonuçları dışarı aktarma](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="28820-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
