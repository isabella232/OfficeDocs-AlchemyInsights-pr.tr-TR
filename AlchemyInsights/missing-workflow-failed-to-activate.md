---
title: Eksik İş Akışı Etkinleştirilemede Başarısız Oldu
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36753816"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="d3361-102">Eksik İş Akışı Etkinleştirilemede Başarısız Oldu</span><span class="sxs-lookup"><span data-stu-id="d3361-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="d3361-103">Microsoft SharePoint site koleksiyonunda, bir listeye veya kitaplıka genel olarak yeniden kullanılabilir bir iş akışı ("Onay - SharePoint 2010" gibi) ekemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="d3361-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="d3361-104">Bu sorunu gidermek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="d3361-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="d3361-105">SharePoint Designer 2013'te site koleksiyonunun kök web sitesini açın.</span><span class="sxs-lookup"><span data-stu-id="d3361-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="d3361-106">**Site Nesneleri** **altında, İş Akışları'nı**seçin.</span><span class="sxs-lookup"><span data-stu-id="d3361-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="d3361-107">**İş Akışları** şeridinin **Yeni** bölümünde, Yeniden Kullanılabilir **İş Akışı'nı**seçin.</span><span class="sxs-lookup"><span data-stu-id="d3361-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="d3361-108">Yeniden **Kullanılabilir İş Akışı Oluştur** formuna \*\* *Repair2010* \*\*adını girin.</span><span class="sxs-lookup"><span data-stu-id="d3361-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="d3361-109">**Platform Türü**için **SharePoint 2010 İş Akışı'nı**tıklatın ve ardından **Tamam'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d3361-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="d3361-110">**İş Akışı** şeridinin **Kaydet** bölümünde **Yayımla'yı**seçin.</span><span class="sxs-lookup"><span data-stu-id="d3361-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="d3361-111">**İş Akışı** şeridinin **Yönet** bölümünde, Genel **Olarak Yayımla'yı**seçin.</span><span class="sxs-lookup"><span data-stu-id="d3361-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="d3361-112">Görünen onay iletişim kutusunda **Tamam'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="d3361-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="d3361-113">Bir web tarayıcısında, site koleksiyonunun kök web sitesini bulun ve **ardından Site Ayarları** \> **Site Toplama Özelliklerine**erişin.</span><span class="sxs-lookup"><span data-stu-id="d3361-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="d3361-114">Ardından, İş **Akışları** özelliğini geçişe:</span><span class="sxs-lookup"><span data-stu-id="d3361-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="d3361-115">· Özellik *Etkinleştirildiyse,* **Devre Dışı bırak'ı** tıklatın ve sonra **Etkinleştir'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d3361-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="d3361-116">· Özellik Devre *Dışı* bırakılırsa, **Etkinleştir'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d3361-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="d3361-117">Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)bakın.</span><span class="sxs-lookup"><span data-stu-id="d3361-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

