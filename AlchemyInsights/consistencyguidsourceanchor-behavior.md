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
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753122"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor davranışı

Azure AD Bağlan (sürüm 1.1.524.0 ve sonra) şimdi sourceAnchor özniteliği olarak msDS-ConsistencyGuid kullanımını kolaylaştırır. Bu özellik kullanılırken, Azure AD Bağlan eşitleme kuralları otomatik olarak yapılandırır:
  
- MsDS-ConsistencyGuid sourceAnchor özniteliği kullanıcı nesneleri için kullanır. ObjectGUID, diğer nesne türleri için kullanılır.
    
- Verilen herhangi için şirket içi AD kullanıcı nesnesi, msDS-ConsistencyGuid özniteliğini objectGUID değerini başa msDS-ConsistencyGuid özniteliği Active Directory'de şirket içi doldurulmuş, Azure AD Bağlan yazma değil. MsDS-ConsistencyGuid özniteliğini yerleştirildikten sonra Azure AD Bağlan sonra Azure AD için nesne dışa aktarır.
    
 **Not:** Bir kez bir şirket içi Reklam nesne (yani AD bağlayıcı alanına alınan ve Metaverse öngörülen) Azure AD Bağlan içine alınır, sourceAnchor değeri artık değiştirilemez. SourceAnchor değerini belirlemek için bir yerinde verilen AD nesne, Azure AD Bağlan alınmadan önce msDS-ConsistencyGuid özniteliği yapılandırın. 
  
Şu şekilde SourceAnchor ve ConsistencyGuid hakkında daha fazla bilgi için bakın: [Azure AD Bağlan: tasarım kavramları](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

