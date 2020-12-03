---
title: Kiracı silme
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564877"
---
# <a name="delete-tenant"></a><span data-ttu-id="100a7-102">Kiracı silme</span><span class="sxs-lookup"><span data-stu-id="100a7-102">Delete tenant</span></span>

<span data-ttu-id="100a7-103">Bir Azure AD silmek için:</span><span class="sxs-lookup"><span data-stu-id="100a7-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="100a7-104">Dizinde genel yöneticisiniz.</span><span class="sxs-lookup"><span data-stu-id="100a7-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="100a7-105">Contoso.onmicrosoft.com gibi varsayılan dizine sahip olan ve admin@contoso.onmicrosoft.com gibi bir hesap ile oturum açmadınız.</span><span class="sxs-lookup"><span data-stu-id="100a7-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="100a7-106">Silmeden önce dizindeki tüm etkin uygulamaları kaldırın.</span><span class="sxs-lookup"><span data-stu-id="100a7-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="100a7-107">Etkin uygulamaları kaldırmak için uygulama kayıtları 'na gidin ve var olan uygulamaları kaldırın.</span><span class="sxs-lookup"><span data-stu-id="100a7-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="100a7-108">Microsoft Azure, Office 365 veya dizinde ilişkilendirilmiş Azure AD Premium gibi herhangi bir Microsoft Online hizmeti için etkin abonelik yoktur.</span><span class="sxs-lookup"><span data-stu-id="100a7-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="100a7-109">Azure desteği ve faturalamayla aboneliklerinizi aktarın veya etkin aboneliklerin iptalini yeniden yapın.</span><span class="sxs-lookup"><span data-stu-id="100a7-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="100a7-110">Office 365 ve Azure aboneliklerini Iptal etme hakkında daha fazla bilgi edinin.</span><span class="sxs-lookup"><span data-stu-id="100a7-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="100a7-111">Bir kiracıya varolan aboneliği ilişkilendirme veya ekleme konusunda rehberlik için [Azure AD kiracınıza Azure aboneliği ilişkilendirme veya ekleme](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="100a7-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="100a7-112">Etkin lisans yok.</span><span class="sxs-lookup"><span data-stu-id="100a7-112">There are no Active license.</span></span> <span data-ttu-id="100a7-113">Lisansları kaldırmak için, [lisansı kaldırma aboneliğini](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)kaldırma konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="100a7-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="100a7-114">Azure AD 'yi silmeye çalışırken, genel yönetici olarak, dizinde başka etkin kullanıcı yok.</span><span class="sxs-lookup"><span data-stu-id="100a7-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="100a7-115">Tüm etkin kullanıcıları kaldırın ve Kiracıdaki özel bir etki alanı adındaki tüm bağımlılıklar, admin@contoso.com ile oluşturulan kullanıcılar gibi de kaldırılmalıdır.</span><span class="sxs-lookup"><span data-stu-id="100a7-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="100a7-116">Bu konuda daha fazla ayrıntı için:</span><span class="sxs-lookup"><span data-stu-id="100a7-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="100a7-117">Azure Active [Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)'yi silme konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="100a7-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="100a7-118">Dizindeki [uygulamaları kaldırmak, bkz.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app)</span><span class="sxs-lookup"><span data-stu-id="100a7-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
