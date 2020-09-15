---
title: 2010 onay Iş akışı eklenemiyor
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699755"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="6680a-102">2010 onay Iş akışı eklenemiyor</span><span class="sxs-lookup"><span data-stu-id="6680a-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="6680a-103">Microsoft SharePoint site koleksiyonunda, bir liste veya kitaplığa genel olarak kullanılabilen bir iş akışı ("onay-SharePoint 2010" gibi) ekleyemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="6680a-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="6680a-104">Bu sorunu çözmek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="6680a-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="6680a-105">SharePoint Designer 2013 'da site koleksiyonunun kök Web sitesini açın.</span><span class="sxs-lookup"><span data-stu-id="6680a-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="6680a-106">**Site nesneleri**altında, **iş akışları**'nı seçin.</span><span class="sxs-lookup"><span data-stu-id="6680a-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="6680a-107">**Iş akışları** şeridinin **Yeni** bölümünde, yeniden **kullanılabilir iş akışı**'nı seçin.</span><span class="sxs-lookup"><span data-stu-id="6680a-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="6680a-108">Yeniden **kullanılabilir Iş akışı oluştur** formunda \* \* *Repair2010* \* \* adını girin.</span><span class="sxs-lookup"><span data-stu-id="6680a-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="6680a-109">**Platform türü**için **SharePoint 2010 iş akışı**'nı ve sonra **Tamam**'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="6680a-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="6680a-110">**Iş akışı** şeridinin **Kaydet** bölümünde **Yayımla**'yı seçin.</span><span class="sxs-lookup"><span data-stu-id="6680a-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="6680a-111">**Iş akışı** şeridinin **Yönet** bölümünde, **genel olarak Yayımla**'yı seçin.</span><span class="sxs-lookup"><span data-stu-id="6680a-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="6680a-112">Görüntülenen onay iletişim kutusunda **Tamam 'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="6680a-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="6680a-113">Web tarayıcısında, site koleksiyonunun kök Web sitesini bulun ve **site ayarları** \> **site koleksiyonu özelliklerine**erişin.</span><span class="sxs-lookup"><span data-stu-id="6680a-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="6680a-114">**Iş akışları** özelliğini değiştirme:</span><span class="sxs-lookup"><span data-stu-id="6680a-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="6680a-115">· Özellik  *etkinleştirilirse*  , **devre dışı bırak** 'ı ve ardından **Etkinleştir**'i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="6680a-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="6680a-116">· Özellik  *devre dışı*  bırakılmışsa **Etkinleştir**'i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="6680a-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="6680a-117">Daha fazla bilgi için lütfen aşağıdaki [makaleye](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)bakın.</span><span class="sxs-lookup"><span data-stu-id="6680a-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

