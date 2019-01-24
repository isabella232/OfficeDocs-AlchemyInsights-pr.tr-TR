---
title: Varsayılan ekleyemezsiniz 2010 onay iş akışı
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29494215"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="eba40-102">Varsayılan ekleyemezsiniz 2010 onay iş akışı</span><span class="sxs-lookup"><span data-stu-id="eba40-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="eba40-103">Bir Microsoft SharePoint site koleksiyonu (örneğin, "onay - SharePoint 2010") genel olarak yeniden kullanılabilir bir iş akışı bir liste veya kitaplığa ekleyemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="eba40-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="eba40-104">Bu sorunu gidermek için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="eba40-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="eba40-105">Kök Web sitesinin site koleksiyonunun SharePoint Designer 2013'de açın.</span><span class="sxs-lookup"><span data-stu-id="eba40-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="eba40-106">**Site nesneleri**altında **iş akışı**seçin.</span><span class="sxs-lookup"><span data-stu-id="eba40-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="eba40-107">**İş akışları** Şerit'in **Yeni** bölümünde, **Yeniden kullanılabilir iş akışı**seçin.</span><span class="sxs-lookup"><span data-stu-id="eba40-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="eba40-p101">**Yeniden kullanılabilir iş akışı Oluştur** formunda, adı girin \* \*\*Repair2010\*\*\*. **Platform türü**, **SharePoint 2010 iş akışını**seçin ve sonra **Tamam**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="eba40-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="eba40-110">**İş akışı** Şerit **Kaydet** bölümünde **Yayımlama**seçin.</span><span class="sxs-lookup"><span data-stu-id="eba40-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="eba40-p102">**Genel olarak yayınlama** **iş akışı** Şerit **Yönet** bölümünde seçin. Görüntülenen onay iletişim kutusunda **Tamam**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="eba40-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="eba40-p103">Bir web tarayıcısında site koleksiyonunun kök Web sitesi bulun ve sonra **Site ayarlarını** erişim \> **Site koleksiyonu özellikleri**. Daha sonra **iş akışı** özelliğini Değiştir:</span><span class="sxs-lookup"><span data-stu-id="eba40-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="eba40-115">· Özellik *etkinleştirildi* , **etkinliğini,** tıklatın ve ardından **Etkinleştir**' i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="eba40-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="eba40-116">· Bu özellik *devre dışı* ise, **Etkinleştir**' i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="eba40-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="eba40-117">Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)bakın.</span><span class="sxs-lookup"><span data-stu-id="eba40-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

