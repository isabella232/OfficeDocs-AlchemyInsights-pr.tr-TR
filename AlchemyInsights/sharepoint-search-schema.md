---
title: SharePoint Online'da arama şemalarını yönetme
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042983"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="316ce-102">SharePoint Online'da arama şemalarını yönetme</span><span class="sxs-lookup"><span data-stu-id="316ce-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="316ce-103">Arama şeması, kullanıcıların neleri arayabildiğini, kullanıcıların nasıl arama yapabileceğini ve sonuçları arama web sitelerinizde nasıl sunabileceğinizi denetler.</span><span class="sxs-lookup"><span data-stu-id="316ce-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="316ce-104">Bkz. [SharePoint Online'da Arama Şemasını yöneterek](https://docs.microsoft.com/sharepoint/manage-search-schema) nasıl yapılacağını öğrenin:</span><span class="sxs-lookup"><span data-stu-id="316ce-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="316ce-105">Arama şemasını değiştirin.</span><span class="sxs-lookup"><span data-stu-id="316ce-105">Change the search schema.</span></span>
- <span data-ttu-id="316ce-106">Yönetilen özellikler oluşturun.</span><span class="sxs-lookup"><span data-stu-id="316ce-106">Create managed properties.</span></span>
- <span data-ttu-id="316ce-107">Harita taranmış harita yönetilen özellikleri sürünerek özellikleri.</span><span class="sxs-lookup"><span data-stu-id="316ce-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="316ce-108">Arama Şemanızın yönetimi yle ilgili olarak aşağıdakileri unutmayın:</span><span class="sxs-lookup"><span data-stu-id="316ce-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="316ce-109">Şema değişikliği yapılırken **uygulamanın duraklatılmış olduğunu** belirten bir uyarı alırsanız, bu yalnızca hizmet bakımı gerçekleştiği nden geçicidir.</span><span class="sxs-lookup"><span data-stu-id="316ce-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="316ce-110">24 saatten fazla zaman geçtiyse ve uyarıyı yaşamaya devam ediyorsanız, lütfen bir destek örneğini kaydedin.</span><span class="sxs-lookup"><span data-stu-id="316ce-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="316ce-111">Yönetilen özellikleri değiştirdiğinizde veya yenilerini eklediğinizde, değişiklikler yalnızca içerik yeniden tarandıktan sonra etkili olur.</span><span class="sxs-lookup"><span data-stu-id="316ce-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="316ce-112">SharePoint Online'da tarama, tanımlanan tarama zamanlamasına bağlı olarak otomatik olarak gerçekleşir.</span><span class="sxs-lookup"><span data-stu-id="316ce-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="316ce-113">Değişikliklerinizin tarandığından emin olmak için, [özellikle listenin veya kitaplığın yeniden dizine ekininin istenmesini isteyebilirsiniz](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="316ce-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="316ce-114">Arama Şeması'na tam bir genel bakış için [bkz.](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="316ce-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


