---
title: Uygulamaları geliştirme sorunları
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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013444"
---
# <a name="issues-developing-applications"></a>Uygulamaları geliştirme sorunları

E-posta (AD) uygulamaları Azure Active Directory en yaygın sorunları gidermek için aşağıdaki makalelere bakın:

- [Yalnızca Chrome tarayıcısını kullanarak uygulamada oturum a açılırken sorun görüyorum](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Uygulamam için belirteç yaşam süresi varsayılanlarını nasıl değiştir olduğumu bilmiyorum](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Uygulama izninin çalışma konusunda kafam karışmış](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Uygulamama nasıl izin ver olduğumu bilmiyorum](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Temsilci ile uygulama izinleri arasındaki farkı anlamadım](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Azure Active Directory Authentication Library (ADAL) ve Azure AD Graph API (AAD Graph) için destek sonu***

- 30 Haziran 2020'den itibaren Azure Active Directory Authentication Library (ADAL) ve Azure AD Graph API'ye (AAD Graph) artık yeni özellikler eklemeyeceğiz. Teknik destek ve güvenlik güncellemeleri sağlamaya devam edeceğiz, ancak artık özellik güncellemeleri sunmayacağız.

- 30 Haziran 2022'den itibaren, ADAL ve AAD Grafiği için desteği sona erdireceğiz ve artık teknik destek veya güvenlik güncellemeleri sunmayacağız. Bu koşul sonucunda, aşağıdakiler olası sonuçları içerir:

    - Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar bu süreden sonra çalışmaya devam edecek ancak herhangi bir teknik destek veya güvenlik güncellemesi almayacaktır.

    - AAD Graph kullanan uygulamalar bu sürenin ardından artık AAD Graph uç Graph almayabilirsiniz

**ADAL Geçişi**

Microsoft uygulamaları kullanıyorsanız, en son özellikleri ve güvenlik güncelleştirmelerini kullanan Microsoft Kimlik Doğrulama Kitaplığı'nın (MSAL) güncelleştirmesini öneririz. Bu öneri, Microsoft'un destek bitiş tarihine kadar uygulamalarını MSAL'a uygulama uygulama işlemini başlatan bağlamındadır. 

Microsoft'un MSAL uygulamalarına geçişi, uygulamaların MSAL'ın devam eden güvenlik ve özellik geliştirmelerinden yararlanmasını sağlar.

1. [ADAL SSS bölümünü okuyunuz](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Uygulamaları platforma göre nasıl taşıyacağınız hakkında bilgi edinin](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Uygulamalardan hangilerinin ADAL'ı kullanabileceğini anlamanız için yardıma ihtiyacınız varsa, tüm uygulamalarınızı kaynak kodunu gözden geçirmenizi ve varsa tüm bağımsız yazılım satıcılarına (ISV) veya uygulama sağlayıcılarına ulaşmanızı öneririz. Microsoft desteği ayrıca kiracınızdaki Microsoft dışı tüm ADAL uygulamalarının bir listesini de sağlayabilir.

**AAD Graph Geçişi**

AAD Graph kullanan uygulamalar için, AAD uygulamalarınızı Microsoft Graph geçirme yönergelerimizi Graph:

1. [Geçiş kontrol listemiz bir başlangıç noktası sağlar.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
2. Azure uygulama kayıt portalınız, hangi uygulamaların AAD Graph kullandığını gösterir. Uygulamalarınızın tüm kaynak kodunu gözden geçirmenizi ve uygun olması durumda tüm bağımsız yazılım satıcılarına (ISV) veya uygulama sağlayıcılarına ulaşmanızı öneririz. Microsoft desteği, kiracınız için AAD ve kullanım Graph bilgi de sağlar.







