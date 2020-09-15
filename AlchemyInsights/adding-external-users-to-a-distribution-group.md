---
title: Dağıtım grubuna dış Kullanıcı ekleme
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663533"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="b30e4-102">Dağıtım grubuna dış Kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="b30e4-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="b30e4-103">Dağıtım grubuna (DG) dış kişi ekleme iki adımlı bir işlemdir:</span><span class="sxs-lookup"><span data-stu-id="b30e4-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="b30e4-104">Dış Kullanıcı için posta kişisi oluşturma:</span><span class="sxs-lookup"><span data-stu-id="b30e4-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="b30e4-105">Yönetim merkezinde, **Kullanıcılar**  >  [kişiler](https://admin.microsoft.com/adminportal/home#/Contact) sayfasına gidin.</span><span class="sxs-lookup"><span data-stu-id="b30e4-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="b30e4-106">**Kişi ekle**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="b30e4-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="b30e4-107">Kişinizin bilgilerini yazın ve **Ekle**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="b30e4-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="b30e4-108">DG 'inize posta kişisi ekleme:</span><span class="sxs-lookup"><span data-stu-id="b30e4-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="b30e4-109">Yönetim merkezinde, **gruplar**  >  [gruplar](https://admin.microsoft.com/adminportal/home#/groups) sayfasına gidin.</span><span class="sxs-lookup"><span data-stu-id="b30e4-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="b30e4-110">Dış kullanıcıyı eklemek istediğiniz DG 'yi bulun ve düzenleme iletişim kutusunu açmak için seçin.</span><span class="sxs-lookup"><span data-stu-id="b30e4-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="b30e4-111">**Üyeler** sekmesinde, **Tümünü görüntüle ve üyeleri Yönet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="b30e4-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="b30e4-112">**Üye Ekle**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="b30e4-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="b30e4-113">Önceki adımda oluşturduğunuz posta kişisini seçin ve ardından **Kaydet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="b30e4-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="b30e4-114">Bu adımları uyguladıktan sonra, dış kullanıcılarınız DG 'ye e-posta gönderemezse veya e-posta almadığınızda, DG yalnızca iç kullanıcılardan gelen e-postalara izin verecek şekilde işaretlenmiş olabilir.</span><span class="sxs-lookup"><span data-stu-id="b30e4-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="b30e4-115">Bu yapılandırmayı denetleyebilir ve [buradaki](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)yönergeleri takip edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b30e4-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="b30e4-116">**Not:** Grubunuzun türü "dağıtım grubu" yerine "Microsoft 365 Grubu" olduğunda bu yönergeler uygulanmaz.</span><span class="sxs-lookup"><span data-stu-id="b30e4-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="b30e4-117">Bu durumda, dış kullanıcıyı doğrudan gruba ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b30e4-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="b30e4-118">Microsoft 365 Groups konuklarına ilişkin ayrıntılı bilgi ve dış konuklar ekleme yönergeleri [Bu makalede](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)bulunabilir.</span><span class="sxs-lookup"><span data-stu-id="b30e4-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  