---
title: SharePoint çevrimiçi arama sözlüklerde yönetme
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 89db349189584a45c54c9c08d37ab669c3c7a39b
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716491"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="9e6d0-102">SharePoint çevrimiçi arama şemayı yönetmek</span><span class="sxs-lookup"><span data-stu-id="9e6d0-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="9e6d0-103">Hangi kullanıcıların arama yapabilmesi için kullanıcılar bunu nasıl arayabilir ve sonuçları, arama sitelerinde ne sunabilir arama şeması denetler.</span><span class="sxs-lookup"><span data-stu-id="9e6d0-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="9e6d0-104">Arama şema değiştirme, yönetilen özellikler oluşturmak ve gezinilen özellikleri yönetilen özelliklerle eşlemek için [SharePoint çevrimiçi arama şeması](https://docs.microsoft.com/en-us/sharepoint/manage-search-schema)bkz.</span><span class="sxs-lookup"><span data-stu-id="9e6d0-104">To change the search schema, create managed properties, and map crawled properties to managed properties, see [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-search-schema).</span></span> <span data-ttu-id="9e6d0-105">Bir şema değişikliği yaparken 'uygulama duraklatıldı' bir uyarı alırsanız, yalnızca geçici olduğundan budur Bakım hizmeti gerçekleşen.</span><span class="sxs-lookup"><span data-stu-id="9e6d0-105">If you receive a warning 'the application is paused' when making a schema change, this is only temporary there is service maintenance occurring.</span></span> 

<span data-ttu-id="9e6d0-106">24 saatten fazla geçmiştir ve uyarı yaşamaya devam ederseniz Lütfen destek durumu günlüğe yazılır.</span><span class="sxs-lookup"><span data-stu-id="9e6d0-106">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>

<span data-ttu-id="9e6d0-107">Yönetilen özelliklerini değiştirmek veya yenilerini eklemek, yalnızca içeriği yeniden gezilen kaldıktan sonra değişiklikler etkili olur.</span><span class="sxs-lookup"><span data-stu-id="9e6d0-107">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="9e6d0-108">Çevrimiçi SharePoint içinde gezinme göre otomatik olarak tanımlanmış gezinme zamanlamaya göre gerçekleşir.</span><span class="sxs-lookup"><span data-stu-id="9e6d0-108">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>

<span data-ttu-id="9e6d0-109">Değişikliklerinizi gezilir emin olmak için özellikle [bir liste veya kitaplığı yeniden dizin oluşturma isteği](https://docs.microsoft.com/en-us/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) olabilir.</span><span class="sxs-lookup"><span data-stu-id="9e6d0-109">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/en-us/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="9e6d0-110">Arama şeması tam bir genel bakış için bkz: [Arama şeması Tanıtımı](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="9e6d0-110">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 

