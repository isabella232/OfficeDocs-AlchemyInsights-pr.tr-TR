---
title: SharePoint Online 'da arama şemasını yönetme
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770571"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="819d0-102">SharePoint Online 'da arama şemasını yönetme</span><span class="sxs-lookup"><span data-stu-id="819d0-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="819d0-103">Arama şeması kullanıcıların neler araybileceklerini, kullanıcıların nasıl arayabilirim ve sonuçları arama Web sitelerinizle nasıl sunabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="819d0-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="819d0-104">Aşağıdakileri yapmayı öğrenmek için [SharePoint Online 'Da arama şemasını yönetme](https://docs.microsoft.com/sharepoint/manage-search-schema) konusuna bakın:</span><span class="sxs-lookup"><span data-stu-id="819d0-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="819d0-105">Arama şemasını değiştirin.</span><span class="sxs-lookup"><span data-stu-id="819d0-105">Change the search schema.</span></span>
- <span data-ttu-id="819d0-106">Yönetilen özellikler oluşturun.</span><span class="sxs-lookup"><span data-stu-id="819d0-106">Create managed properties.</span></span>
- <span data-ttu-id="819d0-107">Gezinilen harita Gezilen özelliklerini yönetilen özellikler 'e eşleyin.</span><span class="sxs-lookup"><span data-stu-id="819d0-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="819d0-108">Arama şemanızı yönetmeye dikkat edin:</span><span class="sxs-lookup"><span data-stu-id="819d0-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="819d0-109">Bir şema değişikliği yapılırken **uygulamanın duraklatıldığını** belirten bir uyarı alırsanız, bu yalnızca hizmet bakımı yapılırken geçicidir.</span><span class="sxs-lookup"><span data-stu-id="819d0-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="819d0-110">24 saatten uzun bir süreyi geçmişse ve hala uyarıyı yaşamaya devam ediyorsanız, lütfen bir destek durumu günlüğe yazılır.</span><span class="sxs-lookup"><span data-stu-id="819d0-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="819d0-111">Yönetilen özellikleri değiştirdiğinizde veya yenilerini eklerseniz, değişiklikler yalnızca içerik yeniden gezilecek şekilde etkinleşir.</span><span class="sxs-lookup"><span data-stu-id="819d0-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="819d0-112">SharePoint Online 'da gezinme, tanımlanan gezinme zamanlamasına göre otomatik olarak gerçekleşir.</span><span class="sxs-lookup"><span data-stu-id="819d0-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="819d0-113">Değişikliklerinizin gezinildiği emin olmak için, özellikle [liste veya kitaplığın yeniden dizinini](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) oluşturabilirsiniz</span><span class="sxs-lookup"><span data-stu-id="819d0-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="819d0-114">Arama şemasına eksiksiz bir genel bakış için [arama şeması](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/) oluşturma konusuna bakın</span><span class="sxs-lookup"><span data-stu-id="819d0-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


