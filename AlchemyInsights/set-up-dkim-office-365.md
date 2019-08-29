---
title: Office 365 DKIM Kurulumu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666284"
---
# <a name="setup-dkim-in-office-365"></a>Office 365 DKIM Kurulumu

Office 365'te özel etki alanları için yapılandırma DKIM tam talimatları [burada](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Özel **her** etki alanı için **iki** DKIM CNAME kayıtlarını etki alanınızın DNS barındırma hizmeti (genellikle, etki alanı Kaydedicisi) oluşturmanız gerekir. Örneğin, contoso.com ve fourthcoffee.com dört DKIM CNAME kaydı gerektirir: iki contoso.com ve iki fourthcoffee.com.

   DKIM CNAME kayıtları özel **her** etki alanı için aşağıdaki biçimi kullanın:

   - **Ana bilgisayar adı**:`selector1._domainkey.<CustomDomain>`

     **Adresine veya değer noktaları**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Ana bilgisayar adı**:`selector2._domainkey.<CustomDomain>`

     **Adresine veya değer noktaları**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> sol tarafındaki metin `.mail.protection.outlook.com` , özelleştirilmiş MX kaydında özel etki alanı (örneğin, `contoso-com` contoso.com etki alanı). \<InitialDomain\> Office 365 (örneğin, contoso.onmicrosoft.com) için kaydolurken kullandığınız etki alanıdır.

2. CNAME kayıtları için özel etki alanlarınızı oluşturduktan sonra aşağıdaki yönergeleri izleyin:

   bir. Sahip olduğunuz iş veya okul hesabı ile [Office 365'te oturum açın](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4).

   b. Sol üst köşedeki uygulama başlatıcı simgesini seçin ve sonra da **Yönetici**'yi seçin.

   c. Sol gezinti, **Yönetim** ' i genişletin ve **Exchange**seçin.

   d. **Koruma**Git > **DKIM**.

   e. Etki alanını seçin ve sonra **etkinleştirmek** için **oturum DKIM imza ile bu etki alanı için iletileri**seçin. Özel her etki alanı için bu adımı yineleyin.
