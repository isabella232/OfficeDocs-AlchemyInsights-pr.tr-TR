---
title: Raporları açmak için eski iletişim kutularının eklemeyi etkinleştirme
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814284"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="d74e4-102">Raporları açmak için eski iletişim kutularının eklemeyi etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="d74e4-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="d74e4-103">**Belirti**</span><span class="sxs-lookup"><span data-stu-id="d74e4-103">**Symptom**</span></span>

<span data-ttu-id="d74e4-104">Kullanıcılar raporları açamıyor.</span><span class="sxs-lookup"><span data-stu-id="d74e4-104">Users are unable to open reports.</span></span> <span data-ttu-id="d74e4-105">"Bir sorun çıktı.</span><span class="sxs-lookup"><span data-stu-id="d74e4-105">"Something has gone wrong.</span></span> <span data-ttu-id="d74e4-106">Daha fazla ayrıntı için teknik ayrıntıları kontrol edin."</span><span class="sxs-lookup"><span data-stu-id="d74e4-106">Check technical details for more details."</span></span>

<span data-ttu-id="d74e4-107">**Neden**</span><span class="sxs-lookup"><span data-stu-id="d74e4-107">**Cause**</span></span>

<span data-ttu-id="d74e4-108">Raporlar UCI'de "Form tanımlayıcı null veya tanımlanmamış" hatasıyla yük aamıyor.</span><span class="sxs-lookup"><span data-stu-id="d74e4-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="d74e4-109">UCI'daki raporlar için hala eski iletişim kutuları gerekir, bu nedenle müşterinin sisteminde *allowlegacydialogbedding* etkin olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="d74e4-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="d74e4-110">**Çözüm**</span><span class="sxs-lookup"><span data-stu-id="d74e4-110">**Solution**</span></span>

1. <span data-ttu-id="d74e4-111">Ayarlar ve **Yönetim >, sistem > ve Genel > gidin.**</span><span class="sxs-lookup"><span data-stu-id="d74e4-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="d74e4-112">"Birleşik Arabirim tarayıcı istemcisinde bazı eski iletişim kutularının eklemesini etkinleştir" seçeneğini Evet olarak **ayarlayın.**</span><span class="sxs-lookup"><span data-stu-id="d74e4-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
