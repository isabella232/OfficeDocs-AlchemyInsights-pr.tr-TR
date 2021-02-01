---
title: Kimlik Doğrulama Kitaplıkları ile ilgili sorunlar
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063702"
---
# <a name="issues-with-authentication-libraries"></a>Kimlik Doğrulama Kitaplıkları ile ilgili sorunlar

1. [Microsoft kimlik platformu kimlik doğrulama kitaplıkları,](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) Microsoft tarafından desteklenen ve uyumlu istemci ve orta yazılım kitaplıklarını listeler.
2. Microsoft Kimlik Doğrulama Kitaplığı (MSAL), farklı uygulama [senaryolarında kullanmak](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) üzere çeşitli kimlik doğrulama akışlarını destekler.
3. Belirteçlerin kimliğini doğrulamak ve almak için, kodundaki yeni bir genel veya gizli istemci uygulamasını başlatmış olursunuz. Microsoft Kimlik Doğrulama Kitaplığı'nın (MSAL) istemci uygulamasını başlatılırken çeşitli yapılandırma seçenekleri ayarekleyebilirsiniz. Daha fazla bilgi edinmek için [bkz. Uygulama yapılandırma seçenekleri.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Azure Active Directory Kimlik Doğrulama Kitaplığı (ADAL) ve Azure AD Graph API'si (AAD Graph) için destek sonu**

**30 Haziran 2020'den** itibaren artık ADAL ve Azure AD Graph'e yeni özellikler eklemeyecek. Teknik destek ve güvenlik güncellemeleri sağlamaya devam edeceğiz, ancak artık özellik güncellemeleri sunmayacağız.

**30 Haziran 2022'den** başlayarak, ADAL ve Azure AD Graph desteğini sona erecek ve artık teknik destek veya güvenlik güncelleştirmeleri sağmayacak.

Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar bu sürenin ardından çalışmaya devam edecektir, ancak teknik destek *veya güvenlik güncelleştirmelerini almayacaktır.*

Bu sürenin ardından Azure AD Graph kullanan uygulamalar artık Azure AD Graph uç noktasının yanıtlarını almayabilirsiniz.

**ADAL Geçişi**

En son özelliklere ve güvenlik güncellemelerine sahip olan [Microsoft Kimlik Doğrulama Kitaplığı'na (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) güncelleme yapmanızı öneririz.

Microsoft uygulamalarını kullanıyorsanız, Microsoft'un son destek bitiş tarihine kadar uygulamalarını MSAL'a geçmektedir ve MSAL'ın devam eden güvenlik ve özellik geliştirmelerinden yararlanacaklarından da temin edin.

Daha fazla bilgi için bkz.:

1. [ADAL SSS bölümünü okuyunuz](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Uygulamaları platforma göre nasıl taşıyacağınız hakkında bilgi edinin](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Uygulamalardan hangilerinin ADAL'ı kullanabileceğini anlamanız için yardıma ihtiyacınız varsa tüm uygulamalarınızı kaynak kodunu gözden geçirmenizi ve varsa tüm ISV'lere veya uygulama sağlayıcılarına ulaşmanızı öneririz. Microsoft desteği ayrıca kiracınızdaki Microsoft dışı tüm ADAL uygulamalarının bir listesini de sağlayabilir.

**AAD Graph Geçişi**

Azure AD Graph kullanan uygulamalar için, Azure AD Graph uygulamalarını Microsoft Graph'e geçirme [yönergelerimizi izleyin.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Geçiş denetim listemiz bir başlama noktası sağlar.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Azure uygulama kayıt portalınız, hangi uygulamaların AAD Graph kullandığını gösterir. Tüm uygulamalarınızın kaynak kodunu gözden geçirmenizi ve uygunsa, herhangi bir ISV veya uygulama sağlayıcıya ulaşmanızı öneririz. Microsoft desteği, kiracınız için tüm AAD Graph kullanımının bir listesini de sağlar.
3. Uygulamanın Microsoft Graph'te verilere erişmesi için, kullanıcı veya yöneticinin izin süreci aracılığıyla ona doğru izinleri ataması gerekir. [Microsoft Graph izinleri başvurusu,](https://docs.microsoft.com/graph/permissions-reference) her bir önemli Microsoft Graph API'leri kümesiyle ilişkilendirilmiş izinleri listeler. Ayrıca, izinleri kullanma konusunda da yol göstermeyi sağlar.
