---
title: API'lerle uygulama geliştirme sorunları
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
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013480"
---
# <a name="issues-developing-applications-with-apis"></a>API'lerle uygulama geliştirme sorunları

AZURE ACTIVE DIRECTORY GRAPH API'sini kullanmaya başlamak için [Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) hızlı başlangıç kılavuzuna bakın veya etkileşimli Azure AD Graph API başvuru belgelerini [inceleyin.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Azure Active Directory Authentication Library (ADAL) ve Azure AD Graph API (AAD Graph) için destek sonu**

**30 Haziran 2020'den** itibaren ADAL ve Azure AD Hizmetleri'ne artık yeni bir özellik Graph. Teknik destek ve güvenlik güncellemeleri sağlamaya devam edeceğiz, ancak artık özellik güncellemeleri sunmayacağız.

**30 Haziran 2022'den** itibaren ADAL ve Azure AD Graph artık teknik destek veya güvenlik güncelleştirmeleri sağlamamayacak.

Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar bu süreden sonra çalışmaya devam edecek ancak herhangi bir teknik destek veya güvenlik güncellemesi almayacaktır.

Azure AD Graph kullanan uygulamalar bu sürenin ardından artık Azure AD Graph uç Graph almayabilirsiniz.

**ADAL Geçişi**

En son özelliklere ve güvenlik güncellemelerine sahip olan [Microsoft Kimlik Doğrulama Kitaplığı'na (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) güncelleme yapmanızı öneririz.

Microsoft uygulamalarını kullanıyorsanız, Microsoft'un destek bitiş tarihine kadar uygulamalarını MSAL'a uygulamalarından MSAL'a en geç geçe kadar işleme devam ettiğini ve MSAL'ın devam eden güvenlik ve özellik geliştirmelerinden yararlanacaklarından, onların da yararlanmasını sağlamayı öğrenin.

1. [ADAL SSS bölümünü okuyun.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Uygulamaları platformlar temelinde geçirme hakkında bilgi edinin.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Uygulamalardan hangilerinin ADAL'ı kullanabileceğini anlamanız için yardıma ihtiyacınız varsa tüm uygulamalarınızı kaynak kodunu gözden geçirmenizi ve varsa tüm ISVs'lere veya uygulama sağlayıcılarına ulaşmanızı öneririz. Microsoft desteği ayrıca kiracınızdaki Microsoft dışı tüm ADAL uygulamalarının bir listesini de sağlayabilir.

**AAD Graph Geçişi**

Azure AD Graph kullanan uygulamalar için, Azure AD Graph uygulamalarını [Microsoft Graph'e geçirme yönergelerimizi Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Geçiş kontrol listemiz bir başlangıç noktası sağlar.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
1. Azure uygulama kayıt portalınız, hangi uygulamaların AAD Graph kullandığını gösterir. Tüm uygulamalarınızın kaynak kodunu gözden geçirmenizi ve uygunsa, herhangi bir ISV veya uygulama sağlayıcıya ulaşmanızı öneririz. Microsoft desteği, kiracınız için tüm AAD kullanım Graph bir liste de sağlar.
1. Uygulamanın Microsoft Graph'deki verilere erişmesi için, kullanıcının veya yöneticinin izin süreci aracılığıyla bu verilere doğru izinleri olması gerekir. Microsoft [Graph izinleri başvurusu,](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) Microsoft kullanıcı api'lerinden her bir ana kümeyle Graph listeler. Ayrıca, izinleri kullanma konusunda yol göstermeyi de sağlar.
