---
title: İş akışı eksik etkinleştirilemedi
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 33b92c2cae1f641b0cd88c82fd4ae5e8632d76c2
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28318454"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="6a80f-102">İş akışı eksik etkinleştirilemedi</span><span class="sxs-lookup"><span data-stu-id="6a80f-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="6a80f-103">Bir Microsoft SharePoint site koleksiyonu (örneğin, "onay - SharePoint 2010") genel olarak yeniden kullanılabilir bir iş akışı bir liste veya kitaplığa ekleyemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="6a80f-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="6a80f-104">Bu sorunu gidermek için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="6a80f-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="6a80f-105">Kök Web sitesinin site koleksiyonunun SharePoint Designer 2013'de açın.</span><span class="sxs-lookup"><span data-stu-id="6a80f-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="6a80f-106">**Site nesneleri**altında **iş akışı**seçin.</span><span class="sxs-lookup"><span data-stu-id="6a80f-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="6a80f-107">**İş akışları** Şerit'in **Yeni** bölümünde, **Yeniden kullanılabilir iş akışı**seçin.</span><span class="sxs-lookup"><span data-stu-id="6a80f-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="6a80f-p101">**Yeniden kullanılabilir iş akışı Oluştur** formunda, adı girin \*\* *Repair2010* \*\*. **Platform türü**, **SharePoint 2010 iş akışı**' nı tıklatın ve sonra **Tamam**' ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="6a80f-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="6a80f-110">**İş akışı** Şerit **Kaydet** bölümünde **Yayımlama**seçin.</span><span class="sxs-lookup"><span data-stu-id="6a80f-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="6a80f-p102">**Genel olarak yayınlama** **iş akışı** Şerit **Yönet** bölümünde seçin. Görüntülenen onay iletişim kutusunda **Tamam**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="6a80f-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="6a80f-p103">Bir web tarayıcısında site koleksiyonunun kök Web sitesi bulun ve sonra **Site ayarlarını** erişim \> **Site koleksiyonu özellikleri**. Daha sonra **iş akışı** özelliğini Değiştir:</span><span class="sxs-lookup"><span data-stu-id="6a80f-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="6a80f-115">· Özellik *etkinleştirildi* , **etkinliğini,** tıklatın ve ardından **Etkinleştir**' i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="6a80f-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="6a80f-116">· Bu özellik *devre dışı* ise, **Etkinleştir**' i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="6a80f-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="6a80f-117">Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)bakın.</span><span class="sxs-lookup"><span data-stu-id="6a80f-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

