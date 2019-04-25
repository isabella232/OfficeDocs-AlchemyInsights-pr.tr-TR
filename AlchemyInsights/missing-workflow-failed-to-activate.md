---
title: İş akışı eksik etkinleştirilemedi
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418453"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="2d253-102">İş akışı eksik etkinleştirilemedi</span><span class="sxs-lookup"><span data-stu-id="2d253-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="2d253-103">Bir Microsoft SharePoint site koleksiyonu (örneğin, "onay - SharePoint 2010") genel olarak yeniden kullanılabilir bir iş akışı bir liste veya kitaplığa ekleyemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="2d253-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="2d253-104">Bu sorunu gidermek için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="2d253-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="2d253-105">Kök Web sitesinin site koleksiyonunun SharePoint Designer 2013'de açın.</span><span class="sxs-lookup"><span data-stu-id="2d253-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="2d253-106">**Site nesneleri**altında **iş akışı**seçin.</span><span class="sxs-lookup"><span data-stu-id="2d253-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="2d253-107">**İş akışları** Şerit'in **Yeni** bölümünde, **Yeniden kullanılabilir iş akışı**seçin.</span><span class="sxs-lookup"><span data-stu-id="2d253-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="2d253-108">**Yeniden kullanılabilir iş akışı Oluştur** formunda, adı girin \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="2d253-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="2d253-109">**Platform türü**, **SharePoint 2010 iş akışı**' nı tıklatın ve sonra **Tamam**' ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="2d253-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="2d253-110">**İş akışı** Şerit **Kaydet** bölümünde **Yayımlama**seçin.</span><span class="sxs-lookup"><span data-stu-id="2d253-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="2d253-111">**Genel olarak yayınlama** **iş akışı** Şerit **Yönet** bölümünde seçin.</span><span class="sxs-lookup"><span data-stu-id="2d253-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="2d253-112">Görüntülenen onay iletişim kutusunda **Tamam**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="2d253-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="2d253-113">Bir web tarayıcısında site koleksiyonunun kök Web sitesi bulun ve sonra **Site ayarlarını** erişim \> **Site koleksiyonu özellikleri**.</span><span class="sxs-lookup"><span data-stu-id="2d253-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="2d253-114">Daha sonra **iş akışı** özelliğini Değiştir:</span><span class="sxs-lookup"><span data-stu-id="2d253-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="2d253-115">· Özellik *etkinleştirildi* , **etkinliğini,** tıklatın ve ardından **Etkinleştir**' i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="2d253-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="2d253-116">· Bu özellik *devre dışı* ise, **Etkinleştir**' i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="2d253-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="2d253-117">Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)bakın.</span><span class="sxs-lookup"><span data-stu-id="2d253-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

