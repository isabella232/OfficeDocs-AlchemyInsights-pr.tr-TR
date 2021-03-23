---
title: Kimlik Doğrulama Kitaplıkları ile çalışma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036865"
---
# <a name="working-with-authentication-libraries"></a>Kimlik Doğrulama Kitaplıkları ile çalışma

Microsoft Kimlik Doğrulama Kitaplığı (MSAL) sorununu çözmek için, aşağıdaki önerilen adımları uygulayın:

1. **MSAL :** [Microsoft kimlik platformu kimlik doğrulama kitaplıkları](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) ile çalışma - Bu makalede, çeşitli uygulama türleri için Microsoft Kimlik Doğrulama Kitaplığı desteği açıklanmıştır. Kitaplık kaynak kodunun bağlantılarını içerir; uygulama projenizin paketini nereden edinebilirsiniz; ve kitaplığın kullanıcı oturum açmasını (kimlik doğrulama), korumalı web API'lerine erişimi (yetkilendirme) veya her ikisini birden destekleyip desteklemeyebilirsiniz.

2. **Kimlik Doğrulama Sorunlarını** Giderme: MSAL, farklı uygulama senaryolarında kullanmak üzere çeşitli kimlik doğrulama akışlarını destekler. İstemci uygulamanın nasıl yerleşik olduğunu bağlı olarak, MSAL Microsoft kimlik platformu tarafından desteklenen kimlik doğrulama akışlarından birini veya daha fazlasını kullanabilir. Bu akışlar, çeşitli türde belirteç ve yetkilendirme kodları üretebilirsiniz ve bunların çalışması için farklı belirteçler gerekli olabilir.

3. **Erişim Belirteçleri:** [Microsoft kimlik platformu erişim belirteçleri](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - API'nizin bir erişim belirteci içindeki talepleri nasıl doğrulaya ve kullanabileceğini öğrenin. Bu makaledeki tüm belgeler, not edildi dışındaki yalnızca kayıtlı API'ler için verilen belirteçlere uygulanır. Microsoft'a ait API'ler için verilen belirteçler için geçerli değildir ve bu belirteçler, Microsoft kimlik platformunun sizin oluşturtuz bir API için belirteçleri nasıl çıkartır olacağını doğrulamak için kullanılamaz.

**Azure Active Directory Kimlik Doğrulama Kitaplığı (ADAL) için destek sonu**

- **30 Haziran 2020'den** itibaren artık ADAL ve Azure AD Graph'e yeni özellikler eklemeyecek. Teknik destek ve güvenlik güncellemeleri sağlamaya devam edeceğiz, ancak artık özellik güncellemeleri sunmayacağız.
- **30 Haziran 2022'den başlayarak,** ADAL ve Azure AD Graph desteğini sona erecek ve artık teknik destek veya güvenlik güncelleştirmeleri sağmayacak.
- Mevcut işletim sistemi sürümlerinde ADAL kullanan uygulamalar bu sürenin ardından çalışmaya devam edecektir, ancak teknik destek veya *güvenlik güncelleştirmelerini almayacaktır.*
- Bu sürenin ardından Azure AD Graph kullanan uygulamalar artık Azure AD Graph uç noktalarından yanıt alamaz.

**ADAL Geçişi**

- En son özelliklere ve güvenlik güncelleştirmelerine sahip olan MSAL'a güncelleştirmenizi öneririz.
- Microsoft uygulamalarını kullanıyorsanız, Microsoft'un son destek bitiş tarihine kadar uygulamalarını MSAL'a geçmektedir ve MSAL'ın devam eden güvenlik ve özellik geliştirmelerinden yararlanacaklarından da temin edin.

1. [ADAL SSS bölümünü okuyun.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Uygulamaları platform başına nasıl geçirilir hakkında bilgi edinin.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)
3. Uygulama platformunun kılavuzunu okuduktan sonra başka sorularınız varsa, [Microsoft Q&A'da](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) [azure-ad-adal-deprecation] etiketiyle gönderide bulunabilir veya kitaplığın GitHub deposunda bir sorun açabilirsiniz. Her [kitaplığın](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) repo bağlantıları için **MSAL genel bakış** makalesinde Diller ve çerçeveler bölümüne bakın.
4. **Uygulamalardan hangilerinin ADAL'ı kullanabileceğini** anlamanız için yardıma ihtiyacınız varsa, uygulamalarınızı tüm kaynak kodunu gözden geçirmenizi öneririz. Uygunsa, herhangi bir Bağımsız yazılım satıcılarına (ISV) veya uygulama sağlayıcılarına erişin. Microsoft desteği ayrıca kiracınızdaki Microsoft dışı tüm ADAL uygulamalarının bir listesini de sağlayabilir.







