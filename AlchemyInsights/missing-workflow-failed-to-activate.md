---
title: Eksik İş Akışı Etkinleştirilemede Başarısız Oldu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762121"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="b8184-102">Eksik İş Akışı Etkinleştirilemede Başarısız Oldu</span><span class="sxs-lookup"><span data-stu-id="b8184-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="b8184-103">Microsoft SharePoint site koleksiyonunda, bir listeye veya kitaplıka genel olarak yeniden kullanılabilir bir iş akışı ("Onay - SharePoint 2010" gibi) ekemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="b8184-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="b8184-104">Bu sorunu gidermek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="b8184-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="b8184-105">SharePoint Designer 2013'te site koleksiyonunun kök web sitesini açın.</span><span class="sxs-lookup"><span data-stu-id="b8184-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="b8184-106">**Site Nesneleri** **altında, İş Akışları'nı**seçin.</span><span class="sxs-lookup"><span data-stu-id="b8184-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="b8184-107">**İş Akışları** şeridinin **Yeni** bölümünde, Yeniden Kullanılabilir **İş Akışı'nı**seçin.</span><span class="sxs-lookup"><span data-stu-id="b8184-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="b8184-108">Yeniden **Kullanılabilir İş Akışı Oluştur** formuna \*\* *Repair2010* \*\*adını girin.</span><span class="sxs-lookup"><span data-stu-id="b8184-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="b8184-109">**Platform Türü**için **SharePoint 2010 İş Akışı'nı**tıklatın ve ardından **Tamam'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="b8184-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="b8184-110">**İş Akışı** şeridinin **Kaydet** bölümünde **Yayımla'yı**seçin.</span><span class="sxs-lookup"><span data-stu-id="b8184-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="b8184-111">**İş Akışı** şeridinin **Yönet** bölümünde, Genel **Olarak Yayımla'yı**seçin.</span><span class="sxs-lookup"><span data-stu-id="b8184-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="b8184-112">Görünen onay iletişim kutusunda **Tamam'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="b8184-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="b8184-113">Bir web tarayıcısında, site koleksiyonunun kök web sitesini bulun ve **ardından Site Ayarları** \> **Site Toplama Özelliklerine**erişin.</span><span class="sxs-lookup"><span data-stu-id="b8184-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="b8184-114">Ardından, İş **Akışları** özelliğini geçişe:</span><span class="sxs-lookup"><span data-stu-id="b8184-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="b8184-115">· Özellik *Etkinleştirildiyse,* **Devre Dışı bırak'ı** tıklatın ve sonra **Etkinleştir'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="b8184-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="b8184-116">· Özellik Devre *Dışı* bırakılırsa, **Etkinleştir'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="b8184-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="b8184-117">Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)bakın.</span><span class="sxs-lookup"><span data-stu-id="b8184-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

