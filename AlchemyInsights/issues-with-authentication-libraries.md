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
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028024"
---
# <a name="issues-with-authentication-libraries"></a>Kimlik Doğrulama Kitaplıkları ile ilgili sorunlar

1. [Microsoft kimlik platformu doğrulama kitaplıkları,](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) Microsoft tarafından desteklenen ve uyumlu istemci ve orta yazılım kitaplıklarını listeler.
2. Microsoft Kimlik Doğrulama Kitaplığı (MSAL), farklı uygulama [senaryolarında kullanmak](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) üzere çeşitli kimlik doğrulama akışlarını destekler.
3. Belirteçlerin kimliğini doğrulamak ve almak için, kodunda yeni bir genel veya gizli istemci uygulaması başlatılır. Microsoft Kimlik Doğrulama Kitaplığı'da (MSAL) istemci uygulamasını başlatarak çeşitli yapılandırma seçenekleri de kullanabilirsiniz. Daha fazla bilgi edinmek için [bkz. Uygulama yapılandırma seçenekleri.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Azure Active Directory Authentication Library (ADAL) ve Azure AD Graph API (AAD Graph) için destek sonu**

**30 Haziran 2020'den** itibaren ADAL ve Azure AD Hizmetleri'ne artık yeni bir özellik Graph. Teknik destek ve güvenlik güncellemeleri sağlamaya devam edeceğiz, ancak artık özellik güncellemeleri sunmayacağız.

**30 Haziran 2022'den** itibaren ADAL ve Azure AD Graph artık teknik destek veya güvenlik güncelleştirmeleri sağlamamayacak.

Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar bu sürenin ardından çalışmaya devam edecektir ancak teknik destek *veya güvenlik güncelleştirmelerini almayacaktır.*

Azure AD Graph kullanan uygulamalar bu sürenin ardından artık Azure AD Graph uç Graph almayabilirsiniz.

**ADAL Geçişi**

En son özelliklere ve güvenlik güncellemelerine sahip olan [Microsoft Kimlik Doğrulama Kitaplığı'na (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) güncelleme yapmanızı öneririz.

Microsoft uygulamaları kullanıyorsanız, Microsoft'un destek bitiş tarihine kadar uygulamalarını MSAL'a en geç geçe kadar MSAL'a bölme sürecinde olduğunu ve MSAL'ın devam eden güvenlik ve özellik geliştirmelerinden yararlanacaklarından, onların da yararlanmasını sağlamayı öğrenin.

Daha fazla bilgi için bkz.:

1. [ADAL SSS bölümünü okuyunuz](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Uygulamaları platforma göre nasıl taşıyacağınız hakkında bilgi edinin](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Uygulamalardan hangilerinin ADAL'ı kullanabileceğini anlamanız için yardıma ihtiyacınız varsa tüm uygulamalarınızı kaynak kodunu gözden geçirmenizi ve varsa tüm ISVs'lere veya uygulama sağlayıcılarına ulaşmanızı öneririz. Microsoft desteği ayrıca kiracınızdaki Microsoft dışı tüm ADAL uygulamalarının bir listesini de sağlayabilir.

**AAD Graph Geçişi**

Azure AD Graph kullanan uygulamalar için, Azure AD Graph uygulamalarını [Microsoft Graph'e geçirme yönergelerimizi Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Geçiş denetim listemiz bir başlarken noktası sağlar.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Azure uygulama kayıt portalınız, hangi uygulamaların AAD Graph kullandığını gösterir. Tüm uygulamalarınızın kaynak kodunu gözden geçirmenizi ve uygunsa, herhangi bir ISV veya uygulama sağlayıcıya ulaşmanızı öneririz. Microsoft desteği, kiracınız için tüm AAD kullanım Graph bir liste de sağlar.
3. Uygulamanın Microsoft Graph'deki verilere erişmesi için, kullanıcının veya yöneticinin izin süreci aracılığıyla bu verilere doğru izinleri olması gerekir. Microsoft [Graph izinleri başvurusu,](https://docs.microsoft.com/graph/permissions-reference) Microsoft kullanıcı api'lerinden her bir ana kümeyle Graph listeler. Ayrıca, izinleri kullanma konusunda yol göstermeyi de sağlar.
