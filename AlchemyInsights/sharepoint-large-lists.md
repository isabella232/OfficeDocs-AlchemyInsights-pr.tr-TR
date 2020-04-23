---
title: SharePoint büyük listeleri
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767305"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="0753c-102">SharePoint'te büyük listeler ve kitaplıklarla çalışma</span><span class="sxs-lookup"><span data-stu-id="0753c-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="0753c-103">SharePoint listeleri ve kitaplıkları en fazla 30 milyon öğe içerebilir, ancak 5.000'den fazla öğesi olduğunda, bunlarla çalışmaya çalıştığınızda bir Liste Görünümü Eşik hatası görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0753c-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="0753c-104">Bu eşik hizmetin performansını korumak için belirlenmiştir.</span><span class="sxs-lookup"><span data-stu-id="0753c-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="0753c-105">Değiştirilemez.</span><span class="sxs-lookup"><span data-stu-id="0753c-105">It can't be changed.</span></span> <span data-ttu-id="0753c-106">Bu eşiğe çarpmamak için:</span><span class="sxs-lookup"><span data-stu-id="0753c-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="0753c-107">**Modern kullanın**</span><span class="sxs-lookup"><span data-stu-id="0753c-107">**Use modern**</span></span>

<span data-ttu-id="0753c-108">Birçok öğeyi gösteren görünümler modern deneyimde en iyi şekilde çalışır.</span><span class="sxs-lookup"><span data-stu-id="0753c-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="0753c-109">Klasik deneyimde görebileceğiniz hatalardan kaçınmak için [modern deneyimi kullanın.](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9)</span><span class="sxs-lookup"><span data-stu-id="0753c-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="0753c-110">**Dizin ekleme**</span><span class="sxs-lookup"><span data-stu-id="0753c-110">**Add indexes**</span></span>

<span data-ttu-id="0753c-111">Dizini olmayan bir sütuna göre filtrelediğinizde veya sıraladığınızda bir hata iletisi görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0753c-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="0753c-112">Ayarlar menüsündeki **Liste Ayarları'ndan** el ile [dizin,](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) ardından **Dizin Lenmiş Sütunlar**ekleyin.</span><span class="sxs-lookup"><span data-stu-id="0753c-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="0753c-113">**Liste görünümünü edin**</span><span class="sxs-lookup"><span data-stu-id="0753c-113">**Edit the list view**</span></span>

<span data-ttu-id="0753c-114">Büyük bir listeyle çalışırken bir hata [oluşursa, liste görünümünüzü düzeltin.](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)</span><span class="sxs-lookup"><span data-stu-id="0753c-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="0753c-115">Aşağıdaki dört değişiklik liste görünümü eşik hatalarını kaldırır.</span><span class="sxs-lookup"><span data-stu-id="0753c-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="0753c-116">Tüm hataları kaldırmak için dört değişikliği de yapın.</span><span class="sxs-lookup"><span data-stu-id="0753c-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="0753c-117">Hala hata alıyorsanız, [büyük listeleri ve kitaplıkları yönet'i](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)denetleyin.</span><span class="sxs-lookup"><span data-stu-id="0753c-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="0753c-118">Her iki **İlk'ten sütuna göre** **Sıralama** ve **Sonra sütuna göre sıralama**yok'u seçin.</span><span class="sxs-lookup"><span data-stu-id="0753c-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="0753c-119">**Sütuna göre** hem İlk gruptan **Yok'u,** sonra da **sütuna göre gruplandırmayı**seçin.</span><span class="sxs-lookup"><span data-stu-id="0753c-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="0753c-120">Toplamlar bölümündeki tüm **sütunlar** için **Yok'u** seçin.</span><span class="sxs-lookup"><span data-stu-id="0753c-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="0753c-121">**Sütunlar** bölümünden görüntülenmek için bir sütun hariç tümünü seçin.</span><span class="sxs-lookup"><span data-stu-id="0753c-121">Deselect all but one column for display from the **Columns** section.</span></span>

