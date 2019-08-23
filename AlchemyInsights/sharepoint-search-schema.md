---
title: SharePoint çevrimiçi arama şemayı yönetmek
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 704fb3b682d23220d61192e383d7d80f59f27933
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502827"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="fc89b-102">SharePoint çevrimiçi arama şemayı yönetmek</span><span class="sxs-lookup"><span data-stu-id="fc89b-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="fc89b-103">Hangi kullanıcıların arama yapabilmesi için kullanıcılar bunu nasıl arayabilir ve sonuçları, arama sitelerinde ne sunabilir arama şeması denetler.</span><span class="sxs-lookup"><span data-stu-id="fc89b-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="fc89b-104">[Yönetme SharePoint çevrimiçi arama şemada](https://docs.microsoft.com/sharepoint/manage-search-schema) öğrenmek için bkz: nasıl yapılır:</span><span class="sxs-lookup"><span data-stu-id="fc89b-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="fc89b-105">Arama şema değiştirin.</span><span class="sxs-lookup"><span data-stu-id="fc89b-105">Change the search schema.</span></span>
- <span data-ttu-id="fc89b-106">Yönetilen özellikler oluşturmak.</span><span class="sxs-lookup"><span data-stu-id="fc89b-106">Create managed properties.</span></span>
- <span data-ttu-id="fc89b-107">Gezilen özellikler için yönetilen özellikler gezinilen eşlemi.</span><span class="sxs-lookup"><span data-stu-id="fc89b-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="fc89b-108">Gelince, arama şemasını yönetmek için aşağıdakileri göz önünde bulundurun:</span><span class="sxs-lookup"><span data-stu-id="fc89b-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="fc89b-109">**Uygulama duraklatılmış** bir şema değişikliği yaparken bildiren bir uyarı alırsanız, servis bakım olduğundan bu yalnızca geçici gerçekleşen.</span><span class="sxs-lookup"><span data-stu-id="fc89b-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="fc89b-110">24 saatten fazla geçmiştir ve uyarı yaşamaya devam ederseniz Lütfen destek durumu günlüğe yazılır.</span><span class="sxs-lookup"><span data-stu-id="fc89b-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="fc89b-111">Yönetilen özelliklerini değiştirmek veya yenilerini eklemek, yalnızca içeriği yeniden gezilen kaldıktan sonra değişiklikler etkili olur.</span><span class="sxs-lookup"><span data-stu-id="fc89b-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="fc89b-112">Çevrimiçi SharePoint içinde gezinme göre otomatik olarak tanımlanmış gezinme zamanlamaya göre gerçekleşir.</span><span class="sxs-lookup"><span data-stu-id="fc89b-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="fc89b-113">Değişikliklerinizi gezilir emin olmak için özellikle [bir liste veya kitaplığı yeniden dizin oluşturma isteği](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) olabilir.</span><span class="sxs-lookup"><span data-stu-id="fc89b-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="fc89b-114">Arama şeması tam bir genel bakış için bkz: [Arama şeması Tanıtımı](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="fc89b-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


