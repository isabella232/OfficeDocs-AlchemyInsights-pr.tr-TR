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
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645692"
---
# <a name="setup-dkim"></a>Kurulum DKIM

Microsoft 365'teki özel etki alanları için DKIM yapılandırmak için tam yönergeler [burada.](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)

1. **Her** özel etki alanı için, etki alanınızın DNS barındırma hizmetinde (genellikle etki alanı kayıt şirketi) **iki** DKIM CNAME kaydı oluşturmanız gerekir. Örneğin, contoso.com ve fourthcoffee.com dört DKIM CNAME kaydı gerektirir: ikisi contoso.com için, ikisi fourthcoffee.com için.

   **Her** özel etki alanı için DKIM CNAME kayıtları aşağıdaki biçimleri kullanır:

   - **Ev sahibi adı**:`selector1._domainkey.<CustomDomain>`

     **Adrese veya değere işaret:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Ev sahibi adı**:`selector2._domainkey.<CustomDomain>`

     **Adrese veya değere işaret:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID,\> özel etki alanı `.mail.protection.outlook.com` için özelleştirilmiş MX kaydının solundaki `contoso-com` metindir (örneğin, etki alanı contoso.com için). \<InitialDomain,\> Microsoft 365'e kaydolduğunuzda kullandığınız etki alanıdır (örneğin, contoso.onmicrosoft.com).

2. Özel etki alanlarınızın CNAME kayıtlarını oluşturduktan sonra aşağıdaki yönergeleri tamamlayın:

   A. iş veya okul hesabınızla [Microsoft 365'te oturum açın.](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)

   B. Sol üst köşedeki uygulama başlatıcı simgesini seçin ve ardından **Yönetici**’yi seçin.

   C. Sol alt gezintide, **Yönetici'yi** genişletin ve **Exchange'i**seçin.

   D. **Koruma** > **DKIM**gidin.

   E. Etki alanını seçin ve ardından **DKIM imzaları olan bu etki alanı için Oturum İmza iletilerini** **etkinleştir'i** seçin. Her özel etki alanı için bu adımı yineleyin.
