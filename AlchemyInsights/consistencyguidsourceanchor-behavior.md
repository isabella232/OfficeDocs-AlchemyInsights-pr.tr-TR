---
title: Bir GUID/Sourcetutturucu davranışı
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756303"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="977b5-102">Bir GUID/Sourcetutturucu davranışı</span><span class="sxs-lookup"><span data-stu-id="977b5-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="977b5-103">Azure AD Connect (sürüm 1.1.524.0 ve sonrası) artık msDS-.</span><span class="sxs-lookup"><span data-stu-id="977b5-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="977b5-104">Bu özelliği kullanırken, Azure AD Connect eşitleme kurallarını otomatik olarak yapılandırır:</span><span class="sxs-lookup"><span data-stu-id="977b5-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="977b5-105">Kullanıcı nesneleri için Sourcetutturucu özniteliği olarak msDS-en.</span><span class="sxs-lookup"><span data-stu-id="977b5-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="977b5-106">Diğer nesne türleri için Objectguıd kullanılır.</span><span class="sxs-lookup"><span data-stu-id="977b5-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="977b5-107">MSDS-IEN. Guid özniteliği doldurulmadığı herhangi bir şirket içi ad kullanıcı nesnesi için, Azure AD Connect, objectGUID değerini şirket içi Active Directory 'deki MSDS-ı</span><span class="sxs-lookup"><span data-stu-id="977b5-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="977b5-108">MsDS-IEN GUID özniteliği doldurulduktan sonra, Azure AD Connect ardından nesneyi Azure AD 'ye aktarır.</span><span class="sxs-lookup"><span data-stu-id="977b5-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="977b5-109">**Not:** Şirket içi bir AD nesnesi Azure AD Connect 'e aktarıldıktan sonra (yani, AD Bağlayıcısı alanına içeri aktarılmışsa ve meta</span><span class="sxs-lookup"><span data-stu-id="977b5-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="977b5-110">Belirli bir şirket içi AD nesnesinin Sourcetutturucu değerini belirtmek için, bu öğenin msDS-en</span><span class="sxs-lookup"><span data-stu-id="977b5-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="977b5-111">Sourcetutturucu ve sonraki bilgisayarda, Guid hakkında daha fazla bilgi için aşağıdakilere bakın: [Azure AD Connect: tasarım kavramları](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="977b5-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

