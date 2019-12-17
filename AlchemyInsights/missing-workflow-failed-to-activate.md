---
title: Eksik İş Akışı Etkinleştirilemede Başarısız Oldu
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 3df1ddc1059c4cd6cc3f9f42dc157d20be79a63a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052633"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="d91f9-102">Eksik İş Akışı Etkinleştirilemede Başarısız Oldu</span><span class="sxs-lookup"><span data-stu-id="d91f9-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="d91f9-103">Microsoft SharePoint site koleksiyonunda, bir listeye veya kitaplıka genel olarak yeniden kullanılabilir bir iş akışı ("Onay - SharePoint 2010" gibi) ekemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="d91f9-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="d91f9-104">Bu sorunu gidermek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="d91f9-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="d91f9-105">SharePoint Designer 2013'te site koleksiyonunun kök web sitesini açın.</span><span class="sxs-lookup"><span data-stu-id="d91f9-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="d91f9-106">**Site Nesneleri** **altında, İş Akışları'nı**seçin.</span><span class="sxs-lookup"><span data-stu-id="d91f9-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="d91f9-107">**İş Akışları** şeridinin **Yeni** bölümünde, Yeniden Kullanılabilir **İş Akışı'nı**seçin.</span><span class="sxs-lookup"><span data-stu-id="d91f9-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="d91f9-108">Yeniden **Kullanılabilir İş Akışı Oluştur** formuna \*\* *Repair2010* \*\*adını girin.</span><span class="sxs-lookup"><span data-stu-id="d91f9-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="d91f9-109">**Platform Türü**için **SharePoint 2010 İş Akışı'nı**tıklatın ve ardından **Tamam'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d91f9-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="d91f9-110">**İş Akışı** şeridinin **Kaydet** bölümünde **Yayımla'yı**seçin.</span><span class="sxs-lookup"><span data-stu-id="d91f9-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="d91f9-111">**İş Akışı** şeridinin **Yönet** bölümünde, Genel **Olarak Yayımla'yı**seçin.</span><span class="sxs-lookup"><span data-stu-id="d91f9-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="d91f9-112">Görünen onay iletişim kutusunda **Tamam'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="d91f9-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="d91f9-113">Bir web tarayıcısında, site koleksiyonunun kök web sitesini bulun ve **ardından Site Ayarları** \> **Site Toplama Özelliklerine**erişin.</span><span class="sxs-lookup"><span data-stu-id="d91f9-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="d91f9-114">Ardından, İş **Akışları** özelliğini geçişe:</span><span class="sxs-lookup"><span data-stu-id="d91f9-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="d91f9-115">· Özellik *Etkinleştirildiyse,* **Devre Dışı bırak'ı** tıklatın ve sonra **Etkinleştir'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d91f9-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="d91f9-116">· Özellik Devre *Dışı* bırakılırsa, **Etkinleştir'i**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="d91f9-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="d91f9-117">Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)bakın.</span><span class="sxs-lookup"><span data-stu-id="d91f9-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

