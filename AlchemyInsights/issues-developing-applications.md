---
title: Uygulama geliştirme sorunları
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974764"
---
# <a name="issues-developing-applications"></a>Uygulama geliştirme sorunları

Azure Active Directory (AD) uygulamalarını oluştururken sık karşılaşılan sorunları gidermek için aşağıdaki makalelere bakın:

- [Uygulamada yalnızca Chrome tarayıcısını kullanarak oturum açarken sorun yaşıyorum](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Uygulamam için belirteç yaşam süresi varsayılanlarını nasıl değiştireceğinizi bilmiyorum](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Uygulama izninin nasıl çalıştığı hakkında konuşdum](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Uygulamama izin vermeyi bilmiyorum](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Temsilci ile uygulama izinleri arasındaki farkı anlayamıyorum](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Azure Active Directory kimlik doğrulama kütüphanesi (ADAL) ve Azure AD GRAFIĞI API (AAD Graph) _ desteği sonu**

- 30 Haziran 2020 ' de başlıyor, artık Azure Active Directory kimlik doğrulama kitaplığı (ADAL) ve Azure AD grafiği API (AAD Graph) için yeni özellikler ekleyemeyecektir. Teknik destek ve güvenlik güncelleştirmelerini sağlamaya devam edeceğiz ancak artık özellik güncelleştirmeleri sağlamaz.

- 30 Haziran 2022 ' de başlıyor, ADAL ve AAD Graph için desteği sona eririz ve artık teknik destek veya güvenlik güncelleştirmeleri sağlamaz. Bu koşulun sonucu olarak aşağıdaki etkiler:

    - Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar, bu saatten sonra çalışmaya devam edecektir, ancak teknik destek veya güvenlik güncelleştirmelerini alamaz.

    - Bu saatten sonra AAD grafiği kullanan uygulamalar artık AAD grafik uç noktasından yanıt alamıyor

_ *Adal geçişi**

Microsoft uygulamalarını kullanıyorsanız, en son özellikleri ve güvenlik güncelleştirmelerini içeren Microsoft kimlik doğrulama kitaplığı (MSAL) güncelleştirmesini öneririz. Bu öneri, Microsoft 'un uygulamalarını MSAL-of support son tarihine kadar uygulamalarını başlatma işlemini başlatıyor. 

Microsoft 'un uygulamalarını MSAL 'a geçirmek, uygulamaların MSAL 'un devam eden güvenlik ve özellik geliştirmelerinin avantajlarından yararlanmasını sağlar.

1. [ADAL SSS 'sini okuyun](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Uygulamaları platforma göre nasıl geçirebileceğiniz hakkında bilgi edinin](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Hangi uygulamalarınızı ADAL kullanarak kullanacağınızı anlamayla ilgili yardıma ihtiyacınız varsa, tüm uygulamalarınızın kaynak kodunu gözden geçirmenizi ve varsa tüm bağımsız yazılım satıcılarına (ISV 'Ler) veya uygulama sağlayıcılarını gözden geçirmenizi öneririz. Microsoft desteği size kiracınızdaki Microsoft olmayan tüm ADAL uygulamalarının bir listesini sağlayabilir.

**AAD grafik geçişi**

AAD Graph kullanan uygulamalar için, AAD grafik uygulamalarını Microsoft Graph 'a geçirmek için kılavuzumuzu izleyin:

1. [Geçiş denetim listesi başlangıç noktası sağlar](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Azure App Registration Portal 'da, AAD grafiğini kullanan uygulamalar gösterilir. Tüm uygulamalarınızın kaynak kodunu incelemenizi öneririz ve uygulanabiliyorsa, herhangi bir bağımsız yazılım satıcısı (ISV) veya uygulama sağlayıcılarını kullanabilirsiniz. Microsoft destek, kiracınızdaki AAD grafik kullanımıyla ilgili bilgileri de sağlayabilir.







