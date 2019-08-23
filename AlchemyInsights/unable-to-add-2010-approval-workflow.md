---
title: 2010 onay iş akışı eklenemiyor.
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 1f564c5d1e689dcf41b22fab5a05ab1b488c2b0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558637"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="bf240-102">2010 onay iş akışı eklenemiyor.</span><span class="sxs-lookup"><span data-stu-id="bf240-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="bf240-103">Bir Microsoft SharePoint site koleksiyonu (örneğin, "onay - SharePoint 2010") genel olarak yeniden kullanılabilir bir iş akışı bir liste veya kitaplığa ekleyemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="bf240-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="bf240-104">Bu sorunu gidermek için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="bf240-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="bf240-105">Kök Web sitesinin site koleksiyonunun SharePoint Designer 2013'de açın.</span><span class="sxs-lookup"><span data-stu-id="bf240-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="bf240-106">**Site nesneleri**altında **iş akışı**seçin.</span><span class="sxs-lookup"><span data-stu-id="bf240-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="bf240-107">**İş akışları** Şerit'in **Yeni** bölümünde, **Yeniden kullanılabilir iş akışı**seçin.</span><span class="sxs-lookup"><span data-stu-id="bf240-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="bf240-108">**Yeniden kullanılabilir iş akışı Oluştur** formunda, adı girin \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="bf240-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="bf240-109">**Platform türü**, **SharePoint 2010 iş akışı**' nı tıklatın ve sonra **Tamam**' ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="bf240-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="bf240-110">**İş akışı** Şerit **Kaydet** bölümünde **Yayımlama**seçin.</span><span class="sxs-lookup"><span data-stu-id="bf240-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="bf240-111">**Genel olarak yayınlama** **iş akışı** Şerit **Yönet** bölümünde seçin.</span><span class="sxs-lookup"><span data-stu-id="bf240-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="bf240-112">Görüntülenen onay iletişim kutusunda **Tamam**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="bf240-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="bf240-113">Bir web tarayıcısında site koleksiyonunun kök Web sitesi bulun ve sonra **Site ayarlarını** erişim \> **Site koleksiyonu özellikleri**.</span><span class="sxs-lookup"><span data-stu-id="bf240-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="bf240-114">**İş akışı** özelliğini Değiştir:</span><span class="sxs-lookup"><span data-stu-id="bf240-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="bf240-115">· Özellik *etkinleştirildi* , **etkinliğini,** tıklatın ve ardından **Etkinleştir**' i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="bf240-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="bf240-116">· Bu özellik *devre dışı* ise, **Etkinleştir**' i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="bf240-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="bf240-117">Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)bakın.</span><span class="sxs-lookup"><span data-stu-id="bf240-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

