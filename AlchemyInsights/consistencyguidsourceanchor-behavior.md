---
title: TutarlılıkGuid / sourceAnchor davranışı
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36517015"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="4cb7e-102">TutarlılıkGuid / sourceAnchor davranışı</span><span class="sxs-lookup"><span data-stu-id="4cb7e-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="4cb7e-103">Azure AD Connect (sürüm 1.1.524.0 ve sonrası) artık kaynakÇapa özniteliği olarak msDS-ConsistencyGuid kullanımını kolaylaştırır.</span><span class="sxs-lookup"><span data-stu-id="4cb7e-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="4cb7e-104">Azure AD Connect bu özelliği kullanırken eşitleme kurallarını otomatik olarak şu şekilde yapılandırır:</span><span class="sxs-lookup"><span data-stu-id="4cb7e-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="4cb7e-105">MsDS-ConsistencyGuid kullanıcı nesneleri için kaynakÇapa özniteliği olarak kullanın.</span><span class="sxs-lookup"><span data-stu-id="4cb7e-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="4cb7e-106">ObjectGUID diğer nesne türleri için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="4cb7e-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="4cb7e-107">msDS-ConsistencyGuid özniteliği doldurulmayan herhangi bir şirket içi AD Kullanıcı nesnesi için Azure AD Connect objectGUID değerini yerinde Active Directory'deki msDS-ConsistencyGuid özniteliğine geri yazar.</span><span class="sxs-lookup"><span data-stu-id="4cb7e-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="4cb7e-108">msDS-ConsistencyGuid özniteliği doldurulduktan sonra, Azure AD Connect nesneyi Azure AD'ye dışa dışa dışa dışa aktarmaz.</span><span class="sxs-lookup"><span data-stu-id="4cb7e-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="4cb7e-109">**Not:** Şirket içi bir AD nesnesi Azure AD Connect'e alındıktan sonra (diğer bir deyişle, AD Bağlayıcı Sıtkı Alanına aktarıldıktan ve Metaverse'e yansıtıldıktan sonra), kaynağıAnchor değerini artık değiştiremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="4cb7e-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="4cb7e-110">Belirli bir şirket içi AD nesnesinin kaynak Çapa değerini belirtmek için, Azure AD Connect'e aktarılmadan önce msDS-ConsistencyGuid özniteliğini yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="4cb7e-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="4cb7e-111">SourceAnchor ve ConsistencyGuid hakkında daha fazla bilgi için aşağıdakilere bakın: [Azure AD Connect: Tasarım kavramları](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="4cb7e-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

