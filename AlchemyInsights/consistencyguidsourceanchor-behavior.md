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
# <a name="consistencyguid--sourceanchor-behavior"></a>TutarlılıkGuid / sourceAnchor behavior

Azure AD Connect (sürüm 1.1.524.0 ve sonrası) artık msDS-ConsistencyGuid'ın sourceAnchor özniteliği olarak kullanımını kolaylaştırır. Bu özelliği kullanırken, Azure AD Connect eşitleme kurallarını otomatik olarak şu şekilde yapılandırıyor:
  
- Kullanıcı nesneleri için sourceAnchor özniteliği olarak msDS-ConsistencyGuid'ı kullanın. ObjectGUID diğer nesne türleri için kullanılır.
    
- msDS-ConsistencyGuid özniteliği doldurulmamış herhangi bir şirket içi AD Kullanıcı nesnesi için, Azure AD Connect nesneGUID değerini şirket içi Active Directory'de msDS-ConsistencyGuid özniteliğine geri yazar. msDS-ConsistencyGuid özniteliği doldurulduğunda, Azure AD Connect nesneyi Azure AD'ye aktarıyor.
    
 **Not:** Şirket içi AD nesnesi Azure AD Connect'e aktarıldıktan (başka bir ifadeyle, AD Bağlayıcısı Alanı'nın içine aktarılmış ve Metaverse'e projesi) aktarılmışsa, artık sourceAnchor değerini değiştiremezsiniz. Belirli bir şirket içi AD nesnesinin sourceAnchor değerini belirtmek için, Azure AD Connect'e aktarmadan önce msDS-ConsistencyGuid özniteliğini yapılandırın. 
  
SourceAnchor ve ConsistencyGuid hakkında daha fazla bilgi için aşağıdakilere bakın: [Azure AD Connect: Tasarım kavramları](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

