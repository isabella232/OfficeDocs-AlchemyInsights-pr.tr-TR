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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36517015"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>TutarlılıkGuid / sourceAnchor davranışı

Azure AD Connect (sürüm 1.1.524.0 ve sonrası) artık kaynakÇapa özniteliği olarak msDS-ConsistencyGuid kullanımını kolaylaştırır. Azure AD Connect bu özelliği kullanırken eşitleme kurallarını otomatik olarak şu şekilde yapılandırır:
  
- MsDS-ConsistencyGuid kullanıcı nesneleri için kaynakÇapa özniteliği olarak kullanın. ObjectGUID diğer nesne türleri için kullanılır.
    
- msDS-ConsistencyGuid özniteliği doldurulmayan herhangi bir şirket içi AD Kullanıcı nesnesi için Azure AD Connect objectGUID değerini yerinde Active Directory'deki msDS-ConsistencyGuid özniteliğine geri yazar. msDS-ConsistencyGuid özniteliği doldurulduktan sonra, Azure AD Connect nesneyi Azure AD'ye dışa dışa dışa dışa aktarmaz.
    
 **Not:** Şirket içi bir AD nesnesi Azure AD Connect'e alındıktan sonra (diğer bir deyişle, AD Bağlayıcı Sıtkı Alanına aktarıldıktan ve Metaverse'e yansıtıldıktan sonra), kaynağıAnchor değerini artık değiştiremezsiniz. Belirli bir şirket içi AD nesnesinin kaynak Çapa değerini belirtmek için, Azure AD Connect'e aktarılmadan önce msDS-ConsistencyGuid özniteliğini yapılandırın. 
  
SourceAnchor ve ConsistencyGuid hakkında daha fazla bilgi için aşağıdakilere bakın: [Azure AD Connect: Tasarım kavramları](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

