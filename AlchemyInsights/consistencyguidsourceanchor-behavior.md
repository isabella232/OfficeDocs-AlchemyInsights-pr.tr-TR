---
title: TutarlılıkGuid / sourceAnchor behavior
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817012"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="43555-102">TutarlılıkGuid / sourceAnchor behavior</span><span class="sxs-lookup"><span data-stu-id="43555-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="43555-103">Azure AD Connect (sürüm 1.1.524.0 ve sonrası) artık msDS-ConsistencyGuid'ın sourceAnchor özniteliği olarak kullanımını kolaylaştırır.</span><span class="sxs-lookup"><span data-stu-id="43555-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="43555-104">Bu özelliği kullanırken, Azure AD Connect eşitleme kurallarını otomatik olarak şu şekilde yapılandırıyor:</span><span class="sxs-lookup"><span data-stu-id="43555-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="43555-105">Kullanıcı nesneleri için sourceAnchor özniteliği olarak msDS-ConsistencyGuid'ı kullanın.</span><span class="sxs-lookup"><span data-stu-id="43555-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="43555-106">ObjectGUID diğer nesne türleri için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="43555-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="43555-107">msDS-ConsistencyGuid özniteliği doldurulmamış herhangi bir şirket içi AD Kullanıcı nesnesi için, Azure AD Connect nesneGUID değerini şirket içi Active Directory'de msDS-ConsistencyGuid özniteliğine geri yazar.</span><span class="sxs-lookup"><span data-stu-id="43555-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="43555-108">msDS-ConsistencyGuid özniteliği doldurulduğunda, Azure AD Connect nesneyi Azure AD'ye aktarıyor.</span><span class="sxs-lookup"><span data-stu-id="43555-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="43555-109">**Not:** Şirket içi AD nesnesi Azure AD Connect'e aktarıldıktan (başka bir ifadeyle, AD Bağlayıcısı Alanı'nın içine aktarılmış ve Metaverse'e projesi) aktarılmışsa, artık sourceAnchor değerini değiştiremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="43555-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="43555-110">Belirli bir şirket içi AD nesnesinin sourceAnchor değerini belirtmek için, Azure AD Connect'e aktarmadan önce msDS-ConsistencyGuid özniteliğini yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="43555-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="43555-111">SourceAnchor ve ConsistencyGuid hakkında daha fazla bilgi için aşağıdakilere bakın: [Azure AD Connect: Tasarım kavramları](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="43555-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

