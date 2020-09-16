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
# <a name="consistencyguid--sourceanchor-behavior"></a>Bir GUID/Sourcetutturucu davranışı

Azure AD Connect (sürüm 1.1.524.0 ve sonrası) artık msDS-. Bu özelliği kullanırken, Azure AD Connect eşitleme kurallarını otomatik olarak yapılandırır:
  
- Kullanıcı nesneleri için Sourcetutturucu özniteliği olarak msDS-en. Diğer nesne türleri için Objectguıd kullanılır.
    
- MSDS-IEN. Guid özniteliği doldurulmadığı herhangi bir şirket içi ad kullanıcı nesnesi için, Azure AD Connect, objectGUID değerini şirket içi Active Directory 'deki MSDS-ı MsDS-IEN GUID özniteliği doldurulduktan sonra, Azure AD Connect ardından nesneyi Azure AD 'ye aktarır.
    
 **Not:** Şirket içi bir AD nesnesi Azure AD Connect 'e aktarıldıktan sonra (yani, AD Bağlayıcısı alanına içeri aktarılmışsa ve meta Belirli bir şirket içi AD nesnesinin Sourcetutturucu değerini belirtmek için, bu öğenin msDS-en 
  
Sourcetutturucu ve sonraki bilgisayarda, Guid hakkında daha fazla bilgi için aşağıdakilere bakın: [Azure AD Connect: tasarım kavramları](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

