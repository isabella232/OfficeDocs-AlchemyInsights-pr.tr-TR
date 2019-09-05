---
title: Dağıtım Grubuna harici kullanıcı ekleme
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737929"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="c726a-102">Dağıtım Grubuna harici kullanıcı ekleme</span><span class="sxs-lookup"><span data-stu-id="c726a-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="c726a-103">Dağıtım Grubuna (DG) harici bir bağlantı eklemek iki adımlı bir işlemdir:</span><span class="sxs-lookup"><span data-stu-id="c726a-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="c726a-104">Harici kullanıcı için Bir Posta İlgili Kişisi Oluşturun:</span><span class="sxs-lookup"><span data-stu-id="c726a-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="c726a-105">Yönetici merkezinde, **Kullanıcılar** > [Kişileri](https://admin.microsoft.com/adminportal/home#/Contact) sayfasına gidin.</span><span class="sxs-lookup"><span data-stu-id="c726a-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="c726a-106">**Kişi ekle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="c726a-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="c726a-107">İlgili kişinizin bilgilerini yazın ve **Ekle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="c726a-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="c726a-108">Posta İlgili Kişisini DG'nize ekleyin:</span><span class="sxs-lookup"><span data-stu-id="c726a-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="c726a-109">Yönetici merkezinde Gruplar **sayfasına** > [](https://admin.microsoft.com/adminportal/home#/groups) gidin.</span><span class="sxs-lookup"><span data-stu-id="c726a-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="c726a-110">Dış kullanıcıeklemek istediğiniz DG'yi bulun ve edit iletişim kutusunu açmak için seçin.</span><span class="sxs-lookup"><span data-stu-id="c726a-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="c726a-111">**Üyeler** sekmesinde, **Tümünü Görüntüle'yi ve üyeleri yönet'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="c726a-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="c726a-112">**Üye Ekle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="c726a-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="c726a-113">Önceki adımda oluşturduğunuz Posta İlgili Kişisini seçin ve ardından **Kaydet'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="c726a-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="c726a-114">Bu adımları izleyerek dış kullanıcılarınız DG'ye e-posta gönderemezse veya ondan e-posta alamıyorsa, DG yalnızca dahili kullanıcılardan gelen e-postalara izin verecek şekilde işaretlenmiş olabilir.</span><span class="sxs-lookup"><span data-stu-id="c726a-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="c726a-115">Bu yapılandırmayı kontrol edebilir ve [burada](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)yönergeleri izleyerek düzeltebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c726a-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="c726a-116">**Not:** Grubunuzun türü "Dağıtım grubu" yerine "Office 365 grubu" ise bu talimatlar geçerli değildir.</span><span class="sxs-lookup"><span data-stu-id="c726a-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="c726a-117">Bu durumda, dış kullanıcıyı doğrudan Outlook'tan gruba ekleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c726a-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="c726a-118">Office 365 grupları nın konukları hakkında ayrıntılı bilgi ve dış misafir ekleme talimatları [na bu makalede](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)bulunabilir.</span><span class="sxs-lookup"><span data-stu-id="c726a-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  