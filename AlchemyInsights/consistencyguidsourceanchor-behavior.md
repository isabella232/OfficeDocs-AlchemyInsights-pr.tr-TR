---
title: ConsistencyGuid / sourceAnchor davranışı
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
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408128"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="14a78-102">ConsistencyGuid / sourceAnchor davranışı</span><span class="sxs-lookup"><span data-stu-id="14a78-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="14a78-103">Azure AD Bağlan (sürüm 1.1.524.0 ve sonra) şimdi sourceAnchor özniteliği olarak msDS-ConsistencyGuid kullanımını kolaylaştırır.</span><span class="sxs-lookup"><span data-stu-id="14a78-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="14a78-104">Bu özellik kullanılırken, Azure AD Bağlan eşitleme kuralları otomatik olarak yapılandırır:</span><span class="sxs-lookup"><span data-stu-id="14a78-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="14a78-105">MsDS-ConsistencyGuid sourceAnchor özniteliği kullanıcı nesneleri için kullanır.</span><span class="sxs-lookup"><span data-stu-id="14a78-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="14a78-106">ObjectGUID, diğer nesne türleri için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="14a78-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="14a78-107">Verilen herhangi için şirket içi AD kullanıcı nesnesi, msDS-ConsistencyGuid özniteliğini objectGUID değerini başa msDS-ConsistencyGuid özniteliği Active Directory'de şirket içi doldurulmuş, Azure AD Bağlan yazma değil.</span><span class="sxs-lookup"><span data-stu-id="14a78-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="14a78-108">MsDS-ConsistencyGuid özniteliğini yerleştirildikten sonra Azure AD Bağlan sonra Azure AD için nesne dışa aktarır.</span><span class="sxs-lookup"><span data-stu-id="14a78-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="14a78-109">**Not:** Bir kez bir şirket içi Reklam nesne (yani AD bağlayıcı alanına alınan ve Metaverse öngörülen) Azure AD Bağlan içine alınır, sourceAnchor değeri artık değiştirilemez.</span><span class="sxs-lookup"><span data-stu-id="14a78-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="14a78-110">SourceAnchor değerini belirlemek için bir yerinde verilen AD nesne, Azure AD Bağlan alınmadan önce msDS-ConsistencyGuid özniteliği yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="14a78-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="14a78-111">Şu şekilde SourceAnchor ve ConsistencyGuid hakkında daha fazla bilgi için bakın: [Azure AD Bağlan: tasarım kavramları](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="14a78-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

