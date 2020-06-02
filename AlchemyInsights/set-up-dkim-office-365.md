---
title: Kurulum DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509404"
---
# <a name="setup-dkim"></a>Kurulum DKIM

Microsoft 365'teki özel etki alanları için DKIM yapılandırmak için tam yönergeler [burada.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. **Her** özel etki alanı için, etki alanınızın DNS barındırma hizmetinde (genellikle etki alanı kayıt şirketi) **iki** DKIM CNAME kaydı oluşturmanız gerekir. Örneğin, contoso.com ve fourthcoffee.com dört DKIM CNAME kaydı gerektirir: ikisi contoso.com için, ikisi fourthcoffee.com için.

   **Her** özel etki alanı için DKIM CNAME kayıtları aşağıdaki biçimleri kullanır:

   - **Ev sahibi adı**:`selector1._domainkey.<CustomDomain>`

     **Adrese veya değere işaret:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Ev sahibi adı**:`selector2._domainkey.<CustomDomain>`

     **Adrese veya değere işaret:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>`.mail.protection.outlook.com`özel etki alanı için özelleştirilmiş MX kaydında solundaki metindir (örneğin, `contoso-com` etki alanı contoso.com). \<InitialDomain\>Microsoft 365'e kaydolduğunuzda kullandığınız etki alanıdır (örneğin, contoso.onmicrosoft.com).

2. Özel etki alanlarınızın CNAME kayıtlarını oluşturduktan sonra aşağıdaki yönergeleri tamamlayın:

   a. iş veya okul hesabınızla [Microsoft 365'te oturum açın.](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)

   b. Sol üst köşedeki uygulama başlatıcı simgesini seçin ve ardından **Yönetici**’yi seçin.

   c. Sol alt gezintide, **Yönetici'yi** genişletin ve **Exchange'i**seçin.

   D. Koruma **Protection**  >  **DKIM**gidin.

   E. Etki alanını seçin ve ardından **DKIM imzaları olan bu etki alanı için Oturum İmza iletilerini** **etkinleştir'i** seçin. Her özel etki alanı için bu adımı yineleyin.
