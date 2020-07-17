---
title: Kullanıcılarınızın başka bir kuruluşla işbirliği yapmasına izin vermek için bir Kuruluş İlişkisi oluşturma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 2c6cd6a178c6e012bfe1c8d769b037168ffa3254
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862190"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="29b18-102">Kullanıcılarınızın başka bir kuruluşla işbirliği yapmasına izin vermek için bir Kuruluş İlişkisi oluşturma</span><span class="sxs-lookup"><span data-stu-id="29b18-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="29b18-103">Microsoft 365 yönetici merkezi **panosundan, Yönetici**  >  **Exchange'e**gidin.</span><span class="sxs-lookup"><span data-stu-id="29b18-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="29b18-104">Kuruluş **organization**  >  **paylaşımına**gidin.</span><span class="sxs-lookup"><span data-stu-id="29b18-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="29b18-105">**Kuruluş Paylaşımı**altında, **Yeni'yi** tıklatın.</span><span class="sxs-lookup"><span data-stu-id="29b18-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="29b18-106">İlişki **adı** kutusunda, **yeni kuruluş ilişkisinde,** kuruluş ilişkisi için uygun bir ad yazın.</span><span class="sxs-lookup"><span data-stu-id="29b18-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="29b18-107">Kutuyla **paylaşmak üzere Etki Alanları'nda,** takvimlerinizi görmek istediğiniz harici Office 365 veya Exchange şirket içi kuruluşun etki alanını yazın.</span><span class="sxs-lookup"><span data-stu-id="29b18-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="29b18-108">Birden fazla etki alanı girmeniz gerekiyorsa, etki alanı adlarını virgülle ayırın.</span><span class="sxs-lookup"><span data-stu-id="29b18-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="29b18-109">Örneğin, contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="29b18-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="29b18-110">Listelediğiniz etki alanlarıyla takvim paylaşımını açmak için **takvime etkin/meşgul bilgi paylaşımı onay** kutusunu etkinleştir'i seçin.</span><span class="sxs-lookup"><span data-stu-id="29b18-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="29b18-111">Takvim ücretsiz/meşgul bilgileri için paylaşım düzeyini ayarlayın ve kullanıcıların takvim ücretsiz/meşgul bilgilerini paylaşabilecekleri ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="29b18-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="29b18-112">Boş/yoğun erişim düzeyini ayarlamak için aşağıdakilerden birini seçin:</span><span class="sxs-lookup"><span data-stu-id="29b18-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="29b18-113">**Yalnızca zaman ile takvim uygun/meşgul bilgisi**</span><span class="sxs-lookup"><span data-stu-id="29b18-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="29b18-114">**Takvim ücretsiz/zaman, konu ve konumla meşgul**</span><span class="sxs-lookup"><span data-stu-id="29b18-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="29b18-115">Takvim ücretsiz/meşgul bilgilerini hangi kullanıcıların paylaşacağını ayarlamak için aşağıdakilerden birini seçin:</span><span class="sxs-lookup"><span data-stu-id="29b18-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="29b18-116">**Kuruluşunuzdaki herkes**</span><span class="sxs-lookup"><span data-stu-id="29b18-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="29b18-117">**Belirli bir güvenlik grubu**</span><span class="sxs-lookup"><span data-stu-id="29b18-117">**A specified security group**</span></span>  

<span data-ttu-id="29b18-118">Güvenlik grubunu listeden seçmek için **göz atın'ı** tıklatın ve ardından **tamam'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="29b18-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="29b18-119">Kuruluş ilişkisini oluşturmak için **kaydet'i** tıklatın.</span><span class="sxs-lookup"><span data-stu-id="29b18-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="29b18-120">**Not:** Kiracılar arası yapılandırmalar, ücretsiz/yoğun arama için kişisel kişileri desteklemez.</span><span class="sxs-lookup"><span data-stu-id="29b18-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="29b18-121">İlgili kişiler, ücretsiz/yoğun bir şekilde çalışmak için genel adres listesine eklenmelidir.</span><span class="sxs-lookup"><span data-stu-id="29b18-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="29b18-122">**Bu konunun tam olarak anlaşılması için lütfen okuyun:**</span><span class="sxs-lookup"><span data-stu-id="29b18-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="29b18-123">Exchange Online'da bir kuruluş ilişkisi oluşturma</span><span class="sxs-lookup"><span data-stu-id="29b18-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="29b18-124">Exchange Online'da kuruluş ilişkisini değiştirme</span><span class="sxs-lookup"><span data-stu-id="29b18-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="29b18-125">Exchange Online'da bir kuruluş ilişkisini kaldırma</span><span class="sxs-lookup"><span data-stu-id="29b18-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
