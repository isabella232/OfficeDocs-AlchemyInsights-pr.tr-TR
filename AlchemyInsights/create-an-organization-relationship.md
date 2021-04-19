---
title: Kullanıcılarınızı başka bir kuruluşla işbirliği yapmak için Kuruluş İlişkisi oluşturma
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
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816148"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="ec21d-102">Kullanıcılarınızı başka bir kuruluşla işbirliği yapmak için Kuruluş İlişkisi oluşturma</span><span class="sxs-lookup"><span data-stu-id="ec21d-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="ec21d-103">Microsoft 365 yönetim merkezi panosunda Yönetici **Exchange'e**  >  **gidin.**</span><span class="sxs-lookup"><span data-stu-id="ec21d-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="ec21d-104">Kuruluş paylaşımı  >  **'ne gidin.**</span><span class="sxs-lookup"><span data-stu-id="ec21d-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="ec21d-105">Kuruluş **Paylaşımı altında,** Yeni **'ye tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="ec21d-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="ec21d-106">Yeni **kuruluş ilişkisinde,** **İlişki adı kutusuna** kuruluş ilişkisi için kolay bir ad yazın.</span><span class="sxs-lookup"><span data-stu-id="ec21d-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="ec21d-107">Paylaşacağız **etki alanları** kutusuna takvimlerinizi görmelerini istediğiniz dış Office 365 veya Exchange şirket içi kuruluşlarının etki alanını yazın.</span><span class="sxs-lookup"><span data-stu-id="ec21d-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="ec21d-108">Birden fazla etki alanı girmeniz gerekirse, etki alanı adlarını virgülle birbirinden ayırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ec21d-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="ec21d-109">Örneğin, contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="ec21d-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="ec21d-110">Listelenen etki **alanlarıyla takvim paylaşımını açmak için Takvim serbest/meşgul** bilgi paylaşımını etkinleştir onay kutusunu seçin.</span><span class="sxs-lookup"><span data-stu-id="ec21d-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="ec21d-111">Takvim serbest/meşgul bilgisinin paylaşım düzeyini ayarlayın ve hangi kullanıcıların takvim serbest/meşgul bilgilerini paylaşa ayarlaması için bunu ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="ec21d-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="ec21d-112">Serbest/meşgul erişim düzeyini ayarlamak için, aşağıdaki seçeneklerden birini seçin:</span><span class="sxs-lookup"><span data-stu-id="ec21d-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="ec21d-113">**Yalnızca zaman ile takvim uygun/meşgul bilgisi**</span><span class="sxs-lookup"><span data-stu-id="ec21d-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="ec21d-114">**Zaman, konu ve konum ile takvim serbest/meşgul**</span><span class="sxs-lookup"><span data-stu-id="ec21d-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="ec21d-115">Hangi kullanıcıların takvim serbest/meşgul bilgilerini paylaşacaklarını ayarlamak için, aşağıdaki seçeneklerden birini seçin:</span><span class="sxs-lookup"><span data-stu-id="ec21d-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="ec21d-116">**Kuruluşta yer alan herkes**</span><span class="sxs-lookup"><span data-stu-id="ec21d-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="ec21d-117">**Belirtilen bir güvenlik grubu**</span><span class="sxs-lookup"><span data-stu-id="ec21d-117">**A specified security group**</span></span>  

<span data-ttu-id="ec21d-118">Listeden **güvenlik** grubunu seçmek için gözat'a tıklayın ve sonra tamam'a **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="ec21d-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="ec21d-119">Kuruluş **ilişkisini** oluşturmak için Kaydet'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="ec21d-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="ec21d-120">**Not:** Kiracılar arası yapılandırmalar serbest/meşgul araması için kişisel kişileri desteklemez.</span><span class="sxs-lookup"><span data-stu-id="ec21d-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="ec21d-121">Kişilerin serbest/meşgul aramasının çalışması için genel adres listesine ekli olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="ec21d-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="ec21d-122">**Bu konuyu tam olarak anlamak için lütfen aşağıdakini okuyun:**</span><span class="sxs-lookup"><span data-stu-id="ec21d-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="ec21d-123">Exchange Online'da kuruluş ilişkisi oluşturma</span><span class="sxs-lookup"><span data-stu-id="ec21d-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="ec21d-124">Exchange Online'da kuruluş ilişkisini değiştirme</span><span class="sxs-lookup"><span data-stu-id="ec21d-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="ec21d-125">Exchange Online'da kuruluş ilişkisini kaldırma</span><span class="sxs-lookup"><span data-stu-id="ec21d-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
