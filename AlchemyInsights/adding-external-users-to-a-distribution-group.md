---
title: Dış kullanıcı bir dağıtım grubuna ekleme?
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce67797a1838630ab3a42e1eeeefc401a0e3f753
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32398478"
---
# <a name="adding-external-users-to-a-distribution-group"></a><span data-ttu-id="dcd67-102">Dış kullanıcı bir dağıtım grubuna ekleme?</span><span class="sxs-lookup"><span data-stu-id="dcd67-102">Adding external users to a Distribution Group?</span></span>

<span data-ttu-id="dcd67-103">Bir dağıtım grubu (DG) için bir dış kişi ekleme 2 adımlı bir işlemdir:</span><span class="sxs-lookup"><span data-stu-id="dcd67-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="dcd67-104">Dış kullanıcı için bir posta kişi oluşturun:</span><span class="sxs-lookup"><span data-stu-id="dcd67-104">Create a Mail Contact for the external user:</span></span>
    
1. <span data-ttu-id="dcd67-105">Tıklatın Yönetim Portalı kişiyi Düzenle sayfasına gitmek için [Buraya](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="dcd67-105">Click [here](https://admin.microsoft.com/adminportal/home#/Contact) to navigate to the Contact edit page in the Admin portal.</span></span> 
    
2. <span data-ttu-id="dcd67-106">**İlgili Kişi Ekle**seçeneğini tıklatın.</span><span class="sxs-lookup"><span data-stu-id="dcd67-106">Click on **Add a Contact**.</span></span>
    
3. <span data-ttu-id="dcd67-107">İlgili kişinizin bilgileri yazın ve **Kaydet**' i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="dcd67-107">Type the information for your contact and click **Save**.</span></span>
    
2. <span data-ttu-id="dcd67-108">Posta kişi için DG ekleyin:</span><span class="sxs-lookup"><span data-stu-id="dcd67-108">Add the Mail Contact to your DG:</span></span>
    
1. <span data-ttu-id="dcd67-109">' I tıklatın gruplar sayfasına gitmek için [Buraya](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="dcd67-109">Click [here](https://admin.microsoft.com/adminportal/home#/groups) to navigate to the Groups page.</span></span> 
    
2. <span data-ttu-id="dcd67-110">Dış kullanıcı tarafından ekleyin ve üzerinde Düzenle iletişim kutusunu açmak için tıklatın istediğiniz DG bulun.</span><span class="sxs-lookup"><span data-stu-id="dcd67-110">Find the DG you want to add the external user to, and click on it to open the edit dialog.</span></span>
    
3. <span data-ttu-id="dcd67-111">**Üyeler** listesinde **Düzenle** düğmesini tıklatın.</span><span class="sxs-lookup"><span data-stu-id="dcd67-111">Click on the **Edit** button in the **Members** list.</span></span> 
    
4. <span data-ttu-id="dcd67-112">**Üye Ekle**seçeneğini tıklatın.</span><span class="sxs-lookup"><span data-stu-id="dcd67-112">Click on **Add Members**.</span></span>
    
5. <span data-ttu-id="dcd67-113">Önceki adımda oluşturduğunuz posta kişiyi seçin ve **Kaydet**' i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="dcd67-113">Select the Mail Contact you created on the previous step and click **Save**.</span></span>
    
<span data-ttu-id="dcd67-114">Aşağıdaki adımları sonra bile, harici kullanıcılar e-postalar için DG gönderemez veya e-postaları ondan almıyorum, DG e-postalar iç kullanıcıların yalnızca izin vermek üzere işaretlenmiş olabilir.</span><span class="sxs-lookup"><span data-stu-id="dcd67-114">If even after following these steps your external users can't send emails to the DG or don't receive emails from it, it can be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="dcd67-115">Bu yapılandırmayı denetleyin ve yönergeleri izleyerek bu sorunu düzelt [burada](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)</span><span class="sxs-lookup"><span data-stu-id="dcd67-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)</span></span>
  
 <span data-ttu-id="dcd67-116">**Not:** Grubunuzun türü "Dağıtım grubu" yerine "Office 365 grubu" ise bu yönergeler uygulanmaz</span><span class="sxs-lookup"><span data-stu-id="dcd67-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="dcd67-117">Bu durumda, Outlook veya Outlook Web grubuna doğrudan dış kullanıcı ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="dcd67-117">If that is the case, you can add the external user directly to the group from Outlook or Outlook on the Web.</span></span> <span data-ttu-id="dcd67-118">O365 grupları guests hakkında ayrıntılı bir açıklama yanı sıra dış konuklar eklemek için yönergeler [Bu makalede](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)bulunabilir.</span><span class="sxs-lookup"><span data-stu-id="dcd67-118">Detailed explanation on O365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  

