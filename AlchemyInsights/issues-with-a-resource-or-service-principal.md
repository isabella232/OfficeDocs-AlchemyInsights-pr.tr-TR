---
title: Kaynak veya Hizmet Sorumlusu ile ilgili sorunlar
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50714463"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Kaynak veya Hizmet Sorumlusu ile ilgili sorunlar

1. Yeni başlıyorsanız, Azure Active Directory'de uygulama ve hizmet sorumlusu nesneleri [Azure Active Directory'de](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) uygulama kaydı, uygulama nesneleri ve hizmet sorumlularını açıklar: bunların ne olduğu, nasıl kullanıldıkları ve birbirlerine nasıl bağlı olduklarını. Ayrıca, bir uygulamanın uygulama nesnesiyle ilgili hizmet sorumlusu nesneleri arasındaki ilişkiyi göstermek için çok kiracılı bir örnek senaryo da sunulmaktadır.
2. Azure Active Directory'de uygulamaları ve hizmet sorumlusu nesnelerini okuyarak uygulamalar ve hizmet sorumluları [arasındaki ilişki hakkında daha fazla bilgi edinebilirsiniz.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [Nasıl kullanılır:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Kaynaklara erişen bir Azure AD uygulaması ve hizmet sorumlusu oluşturmak için portalın kullanımı, rol tabanlı erişim denetimiyle birlikte 2013'e kadar kullanabileceğiniz yeni bir Azure Active Directory (Azure AD) uygulaması ve hizmet sorumlusu oluşturmanızı gösterir.
4. Hizmet sorumlusu [API'si](https://docs.microsoft.com/graph/api/resources/serviceprincipal)ile, uygulama örneklerini programlı olarak yönetebilir ve bir uygulamanın kiracınız içinde neler yapasını kontrol edin.
5. [servicePrincipal kaynak türü,](https://docs.microsoft.com/graph/api/resources/serviceprincipal) servicePrincipal kaynak türünün tüm özelliklerini ve yöntemlerini listeler.
6. Azure AD Graph ile Microsoft Graph arasındaki kaynak türü [farklılıkları,](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) Azure AD Graph ile Microsoft Graph kaynakları arasındaki farkları vurgular. Farklı adlara sahip veya kullanılabilir kaynaklar gösterir; ayrıca, Microsoft Graph'in beta sürümünde bulunan kaynakları da vurgular, ancak v1.0 sürümünde vurgulanmaz.

**Konuk Kullanıcılarla ilgili sorunlar**

- [Hızlı Başlangıç: Azure portalında](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) dizininize konuk kullanıcı ekleme, Azure portal aracılığıyla Azure AD dizininize yeni bir konuk kullanıcı ekleme, davet gönderme ve konuk kullanıcının davet kullanma işleminin nasıl göründüğünü görmenizi sağlar.
- [Öğretici: Azure Active Directory B2C'de](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) kullanıcı akışları oluşturma, Azure portalını kullanarak önerilen kullanıcı akışlarının nasıl oluşturulacaklarını gösterir. Uygulamanıza kaynak sahibi parola kimlik bilgileri (ROPC) akışı ayarlama hakkında bilgi arıyorsanız, Azure AD B2C'de kaynak sahibi parola kimlik bilgileri akışını yapılandırma.
