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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044361"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>TutarlılıkGuid / sourceAnchor behavior

Azure AD Bağlan (sürüm 1.1.524.0 ve sonrası) artık sourceAnchor özniteliği olarak msDS-ConsistencyGuid kullanımını kolaylaştırır. Bu özelliği kullanırken, Azure AD Bağlan eşitleme kurallarını şu şekilde otomatik olarak yapılandırıyor:
  
- Kullanıcı nesneleri için sourceAnchor özniteliği olarak msDS-ConsistencyGuid'ı kullanın. ObjectGUID diğer nesne türleri için kullanılır.
    
- msDS-ConsistencyGuid özniteliği doldurulmamış herhangi bir şirket içi AD Kullanıcı nesnesi için, Azure AD Bağlan nesneGUID değerini şirket içi Active Directory'de msDS-ConsistencyGuid özniteliğine geri yazar. msDS-ConsistencyGuid özniteliği doldurulduğunda, Azure AD Bağlan nesneyi Azure AD'ye aktarmış olur.
    
 **Not:** Şirket içi AD nesnesi Azure AD Bağlan'e aktarıldıktan (başka bir ifadeyle, AD Bağlayıcısı Alanı'nın içine aktarılmış ve MetaVerse'e projesi) aktarılmışsa, sourceAnchor değerini artık değiştiremezsiniz. Belirli bir şirket içi AD nesnesinin sourceAnchor değerini belirtmek için, Azure AD'ye aktarmadan önce msDS-ConsistencyGuid özniteliğini Bağlan. 
  
SourceAnchor ve ConsistencyGuid hakkında daha fazla bilgi için aşağıdakilere bakın: [Azure AD Bağlan: Tasarım kavramları](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

