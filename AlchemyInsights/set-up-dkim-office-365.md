---
title: DkIM kurulumu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108576"
---
# <a name="setup-dkim"></a>DkIM kurulumu

Microsoft 365'de özel etki alanları için DKIM'i yapılandırma Microsoft 365 [burada.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Her **özel** etki alanı için, etki alanı **DNS** barındırma hizmetnde (normalde etki alanı kayıt şirketi) iki DKIM CNAME kaydı oluşturmanız gerekir. Örneğin, contoso.com ve fourthcoffee.com için dört DKIM CNAME kaydı gerekir: contoso.com ve kayıt için fourthcoffee.com.

   Her özel etki alanı için DKIM CNAME **kayıtları** aşağıdaki biçimleri kullanır:

   - **Ana bilgisayar adı:**`selector1._domainkey.<CustomDomain>`

     **Adrese veya değere göre:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Ana bilgisayar adı:**`selector2._domainkey.<CustomDomain>`

     **Adrese veya değere göre:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> özel etki alanı için özelleştirilmiş MX kaydında (örneğin, etki alanı kayıtlarında) `.mail.protection.outlook.com` `contoso-com` sol tarafta kalan contoso.com. \<InitialDomain\>bu, e-posta için kayıt olurken Microsoft 365 etki alanıdır (örneğin, contoso.onmicrosoft.com).

2. Özel etki alanlarınız için CNAME kayıtlarını oluşturduktan sonra, aşağıdaki yönergeleri izleyin:

   a. [iş veya Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) hesabınızla oturum açın.

   b. Sol üst köşedeki uygulama başlatıcı simgesini seçin ve ardından **Yönetici**’yi seçin.

   c. Sol alt gezintide Yönetici'yi genişletin **ve Sol** **Exchange.**

   d. Protection   >  **DKIM 'ye gidin.**

   e. Etki alanını seçin ve ardından Bu **etki alanı için** iletileri **DKIM imzaları ile imzalama için Etkinleştir'i seçin.** Her özel etki alanı için bu adımı yineler.
