---
title: Dış kullanıcı bir dağıtım grubuna ekleme
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 641636add2069fc395df9af156d8c011493a634a
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/29/2019
ms.locfileid: "36660812"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="82222-102">Harici kullanıcılar bir dağıtım grubuna ekleyin.</span><span class="sxs-lookup"><span data-stu-id="82222-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="82222-103">Bir dağıtım grubu (DG) için harici bir ilgili kişi eklemek iki adımdan oluşan bir işlemdir:</span><span class="sxs-lookup"><span data-stu-id="82222-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="82222-104">Dış kullanıcı için bir posta kişi oluşturun:</span><span class="sxs-lookup"><span data-stu-id="82222-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="82222-105">**Kullanıcıların**Yönetim Merkezi'nde Git > [Kişiler](https://admin.microsoft.com/adminportal/home#/Contact) sayfası.</span><span class="sxs-lookup"><span data-stu-id="82222-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="82222-106">**Kişi Ekle**seçin.</span><span class="sxs-lookup"><span data-stu-id="82222-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="82222-107">İlgili kişinizin bilgileri yazın ve **Ekle**' yi seçin.</span><span class="sxs-lookup"><span data-stu-id="82222-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="82222-108">Posta kişi için DG ekleyin:</span><span class="sxs-lookup"><span data-stu-id="82222-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="82222-109">Yönetim Merkezi'nde **grupları**Git > [Gruplar](https://admin.microsoft.com/adminportal/home#/groups) sayfası.</span><span class="sxs-lookup"><span data-stu-id="82222-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="82222-110">Dış kullanıcı için eklemek istediğiniz DG bulun ve Düzenle iletişim kutusunu açmak için seçin.</span><span class="sxs-lookup"><span data-stu-id="82222-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="82222-111">**Üyeler** sekmesinde, **görüntülemek ve üyeleri Yönet'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="82222-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="82222-112">**Üyeler Ekle**seçin.</span><span class="sxs-lookup"><span data-stu-id="82222-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="82222-113">Önceki adımda oluşturduğunuz posta kişiyi seçin ve sonra **Kaydet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="82222-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="82222-114">Sonra aşağıdaki adımları, harici kullanıcılar e-postalar için DG gönderemez veya e-postaları ondan almıyorum, DG e-postalar iç kullanıcıların yalnızca izin vermek üzere işaretlenmiş olabilir.</span><span class="sxs-lookup"><span data-stu-id="82222-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="82222-115">Bu yapılandırmayı denetleyin ve yönergeleri izleyerek bu sorunu düzelt [burada](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span><span class="sxs-lookup"><span data-stu-id="82222-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="82222-116">**Not:** Grubunuzun türü "Dağıtım grubu" yerine "Office 365 grubu" ise bu yönergeler uygulanmaz</span><span class="sxs-lookup"><span data-stu-id="82222-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="82222-117">Bu durumda, harici kullanıcı grubuna doğrudan Outlook'tan ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="82222-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="82222-118">[Bu makalede](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx), Office 365 grupları guests hakkında ayrıntılı bilgi yanı sıra dış konuklar eklemek için yönergeler bulunabilir.</span><span class="sxs-lookup"><span data-stu-id="82222-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  