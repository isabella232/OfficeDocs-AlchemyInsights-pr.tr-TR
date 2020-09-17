---
title: Kuruluş kurulumu
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
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808727"
---
# <a name="setup-dkim"></a>Kuruluş kurulumu

Microsoft 365 'de özel etki alanları için VSEÇKIM yapılandırması ile ilgili eksiksiz yönergeler [.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. **Her** özel etki alanı için, etkı alanınızın DNS **two** barındırma hizmetinde (genellikle etki alanı kayıt Örneğin, contoso.com ve fourthcoffee.com için dört DKIM CNAME kaydı gerekir: contoso.com için iki ve fourthcoffee.com için iki.

   **Tüm** özel etki alanları için VSEÇKIM CNAME kayıtları aşağıdaki biçimleri kullanır:

   - **Ana bilgisayar adı**: `selector1._domainkey.<CustomDomain>`

     **Adres veya değer noktaları**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Ana bilgisayar adı**: `selector2._domainkey.<CustomDomain>`

     **Adres veya değer noktaları**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>`.mail.protection.outlook.com`özel etki alanı için ÖZELLEŞTIRILMIŞ MX kaydının solundaki metindir (örneğin, `contoso-com` contoso.com). \<InitialDomain\> , Microsoft 365 (örneğin, contoso.onmicrosoft.com) için kaydolduğunuzda kullandığınız etki alanıdır.

2. Özel etki alanlarınız için CNAME kayıtlarını oluşturduktan sonra aşağıdaki yönergeleri tamamlayın:

   a. iş veya okul hesabınızla [Microsoft 365 oturumu açın](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) .

   b. Sol üst köşedeki uygulama başlatıcı simgesini seçin ve ardından **Yönetici**’yi seçin.

   c. Sol alt gezintide **yönetici** 'Yi genişletip **Exchange**'i seçin.

   d. **Protection**'a gidin  >  **DKIM**.

   e. Etki alanını seçin ve ardından **cıkim imzaları ile bu etki alanı Için imza Iletilerini** **Etkinleştir** 'i seçin. Her özel etki alanı için bu adımı uygulayın.
