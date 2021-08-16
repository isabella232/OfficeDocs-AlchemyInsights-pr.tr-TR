---
title: Kaynak veya Hizmet Sorumlusuyla ilgili sorunlar
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
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028096"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Kaynak veya Hizmet Sorumlusuyla ilgili sorunlar

1. Yeni başlıyorsanız, Azure Active Directory'daki uygulama ve hizmet sorumlusu [nesneleri, Azure Active Directory'de](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) uygulama kaydını, uygulama nesnelerini ve hizmet sorumlularını açıklar: bunların ne olduğu, nasıl kullanıldıları ve birbirlerine nasıl ilişkili olduklarını. Ayrıca, uygulama nesnesiyle ilgili hizmet sorumlusu nesneleri arasındaki ilişkiyi göstermek için çok kiracılı bir örnek senaryo da sunulmaktadır.
2. Azure Active Directory'ta uygulamaları ve hizmet sorumlusu nesnelerini okuyarak, uygulamalar ve hizmet [sorumluları arasındaki ilişki hakkında daha fazla Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [Nasıl yapılan:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Portal kullanarak kaynaklara erişen bir Azure AD uygulaması ve hizmet sorumlusu oluşturmak, size rol tabanlı erişim denetimiyle birlikte kullanıla yeni bir Azure Active Directory (Azure AD) uygulaması ve hizmet sorumlusu oluşturma hakkında bilgi sağlar.
4. Hizmet sorumlusu [API'si](https://docs.microsoft.com/graph/api/resources/serviceprincipal)ile uygulama örneklerini programlı olarak yönetebilir ve kiracınız içinde bir uygulamanın neler yapasını kontrol edin.
5. [servicePrincipal kaynak türü,](https://docs.microsoft.com/graph/api/resources/serviceprincipal) servicePrincipal kaynak türünün tüm özelliklerini ve yöntemlerini listeler.
6. [Azure AD Graph Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) arasındaki kaynak türü farklılıkları, Azure AD Graph ile Microsoft Graph vurgular. Farklı adlara sahip veya uygun değil kaynakları gösterir; Ayrıca, Microsoft Graph'in beta sürümünde bulunan ancak v1.0 sürümünde yer alan kaynakları vurgular.

**Konuk Kullanıcılarla ilgili sorunlar**

- [Hızlı Başlangıç: Azure portalında](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) dizininize konuk kullanıcı ekleme, Azure portalı aracılığıyla Azure AD dizininize yeni bir konuk kullanıcı ekleme, davet gönderme ve konuk kullanıcının davet kullanma işleminin nasıl göründüğünü görmenizi sağlar.
- [Öğretici: Microsoft B2C'de kullanıcı](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) akışları Azure Active Directory, Azure portalını kullanarak önerilen kullanıcı akışlarının nasıl oluşturulacaklarını gösterir. Uygulamanıza kaynak sahibi parola kimlik bilgileri (ROPC) akışı ayarlama hakkında bilgi arıyorsanız, bkz. Azure AD B2C'de kaynak sahibi parola kimlik bilgileri akışını yapılandırma.
