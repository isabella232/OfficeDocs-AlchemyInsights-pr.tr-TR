---
title: API ile uygulama geliştirme sorunları
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975021"
---
# <a name="issues-developing-applications-with-apis"></a>API ile uygulama geliştirme sorunları

Azure Active Directory Graph API 'sini kullanmaya başlamak için, [Azure AD GRAFIĞI API hızlı başlangıç kılavuzuna](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) bakın veya [etkileşimli Azure AD grafiği API başvuru belgelerine](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)bakın.

**Azure Active Directory kimlik doğrulama kütüphanesi (ADAL) ve Azure AD grafiği API (AAD grafiği) için destek sonu**

**30 haziran 2020**' de başlıyor, artık adal ve Azure AD grafiğinin yeni özelliklerini eklemeiyoruz. Teknik destek ve güvenlik güncelleştirmelerini sağlamaya devam edeceğiz ancak artık özellik güncelleştirmeleri sağlamaz.

**30 haziran 2022**' de BAŞLıYOR, adal ve Azure AD Graph için desteği son verecek ve artık teknik destek veya güvenlik güncelleştirmeleri sağlayamayacak.

Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar, bu saatten sonra çalışmaya devam edecektir, ancak teknik destek veya güvenlik güncelleştirmelerini alamaz.

Bu saatten sonra Azure AD grafiği kullanan uygulamalar artık Azure AD grafiği uç noktasından yanıt alamaz.

**ADAL geçişi**

En son özellikleri ve güvenlik güncelleştirmelerini içeren [Microsoft kimlik doğrulama kitaplığı (msal)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)güncelleştirmesini öneririz.

Microsoft uygulamalarını kullanıyorsanız, Microsoft 'un uygulamalarını MSAL 'in destek zamanı son tarihine geçirmeyle MSAL devam eden güvenlik ve özellik geliştirmelerinin avantajlarından yararlanabileceği konusunda unutmayın.

1. [Adal SSS 'Sini okuyun](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Uygulamaları tek tek platforma geçirme hakkında bilgi edinin](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Hangi uygulamalarınızı ADAL kullanarak anladığınızdan yardım gerekirse, tüm uygulamalarınızın kaynak kodunu gözden geçirmenizi ve uygulanabiliyorsa, herhangi bir ISV veya uygulama sağlayıcısına ulaşın. Microsoft desteği size kiracınızdaki Microsoft olmayan tüm ADAL uygulamalarının bir listesini sağlayabilir.

**AAD grafik geçişi**

Azure AD grafiği kullanan uygulamalar için, [Azure AD grafiği uygulamalarını Microsoft Graph 'a](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)geçirmek için kılavuzumuzu izleyin.

1. [Geçiş denetim listesi başlangıç noktası sağlar](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Azure App Registration Portal 'da, AAD grafiğini kullanan uygulamalar gösterilir. Tüm uygulamalarınızın kaynak kodunu incelemenizi öneririz ve uygulanabiliyorsa, herhangi bir ISV veya uygulama sağlayıcısına ulaşın. Microsoft desteği size kiracınızdaki tüm AAD grafik kullanımının listesini de verebilir.
1. Uygulamanızın Microsoft Graph 'ta verilere erişmesi için, Kullanıcı veya yöneticinin onay süreci aracılığıyla doğru izinleri vermesi gerekir. [Microsoft Graph Permissions başvurusu](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) , her bir Microsoft Graph API kümesiyle ilişkili izinleri listeler. İzinlerin nasıl kullanılacağı hakkında rehberlik de sağlar.
