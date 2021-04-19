---
title: Kullanıcılarının takvimlerini kuruluş dışındaki kullanıcılarla paylaşmasına olanak sağlayan bir Paylaşım İlkesi oluşturma
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816292"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="a06de-102">Kullanıcılarının takvimlerini kuruluş dışındaki kullanıcılarla paylaşmasına olanak sağlayan bir Paylaşım İlkesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="a06de-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="a06de-103">Microsoft 365 yönetim merkezi panosunda Yönetici **Exchange'e**  >  **gidin.**</span><span class="sxs-lookup"><span data-stu-id="a06de-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="a06de-104">Kuruluş paylaşımı  >  **'ne gidin.**</span><span class="sxs-lookup"><span data-stu-id="a06de-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="a06de-105">Liste görünümünde, Bireysel Paylaşım **altında, Yeni**'ye **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="a06de-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="a06de-106">Yeni **paylaşım ilkesinde,** İlke adı kutusuna paylaşım ilkesi için kolay **bir ad** yazın.</span><span class="sxs-lookup"><span data-stu-id="a06de-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="a06de-107">**İlkenin** paylaşım kurallarını tanımlamak için Ekle'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="a06de-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="a06de-108">Paylaşım **kuralında,** paylaşmak istediğiniz etki alanlarını belirtmek için aşağıdaki seçeneklerden birini belirtin:</span><span class="sxs-lookup"><span data-stu-id="a06de-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="a06de-109">**Tüm etki alanlarıyla paylaşma**</span><span class="sxs-lookup"><span data-stu-id="a06de-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="a06de-110">**Belirli bir etki alanıyla paylaşma**</span><span class="sxs-lookup"><span data-stu-id="a06de-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="a06de-111">Belirli bir **etki alanıyla paylaş'ı** seçin, paylaşmak istediğiniz etki alanının adını yazın.</span><span class="sxs-lookup"><span data-stu-id="a06de-111">If you select **Sharing with a specific domain**, type the name of the domain you want to share with.</span></span> <span data-ttu-id="a06de-112">Bu paylaşım ilkesi için birden çok etki alanı girmeniz gerekirse, ilk etki alanının ayarlarını kaydedin ve daha fazla etki alanı eklemek için paylaşım kurallarını düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="a06de-112">If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="a06de-113">Paylaşılacak bilgileri belirtmek için, Takvim **klasörlerinizi paylaşın** onay kutusunu seçin ve sonra da aşağıdaki seçeneklerden birini belirtin:</span><span class="sxs-lookup"><span data-stu-id="a06de-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="a06de-114">**Yalnızca zaman ile takvim uygun/meşgul bilgisi**</span><span class="sxs-lookup"><span data-stu-id="a06de-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="a06de-115">**Zaman, konu ve konum ile takvim serbest/meşgul bilgisi**</span><span class="sxs-lookup"><span data-stu-id="a06de-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="a06de-116">**Saat, konu, konum ve başlık da dahil olmak üzere tüm takvim randevu bilgileri**</span><span class="sxs-lookup"><span data-stu-id="a06de-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="a06de-117">Paylaşım **ilkesi** kurallarını ayarlamak için kaydet'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="a06de-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="a06de-118">Bu paylaşım ilkenizi, organizasyonum tüm kullanıcılar için yeni varsayılan paylaşım ilkesi olarak ayarlamak için Bu ilkeyi varsayılan paylaşım ilkem yapma **onay** kutusunu seçin.</span><span class="sxs-lookup"><span data-stu-id="a06de-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="a06de-119">Paylaşım **ilkesi** oluşturmak için Kaydet'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="a06de-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="a06de-120">**Bu konuyu tam olarak anlamak için lütfen aşağıdakini okuyun:**</span><span class="sxs-lookup"><span data-stu-id="a06de-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="a06de-121">Exchange Online'da paylaşım ilkesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="a06de-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="a06de-122">Exchange Online'da posta kutularına paylaşım ilkesi uygulama</span><span class="sxs-lookup"><span data-stu-id="a06de-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="a06de-123">Exchange Online'da paylaşım ilkesi değiştirme, devre dışı bırakma veya kaldırma</span><span class="sxs-lookup"><span data-stu-id="a06de-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)