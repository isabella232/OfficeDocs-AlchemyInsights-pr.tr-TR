---
title: DKIM kayıt biçimlendirmesi ile ilgili sık karşılaşılan sorunları düzeltme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750753"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>DKIM kaydı biçimlendirmesi ile ilgili sık karşılaşılan sorunları düzeltme

DKIM ayarlama sorunlarının çoğu hatalı DNS kayıtlarıyla ilgilidir.

DKIM ayarlama sorunlarını düzeltmek için DKIM CNAME kaydının **(TXT** kaydı değil) doğru biçimlendirilmiş olduğunu doğrulayın. Daha fazla bilgi için [Bkz. Office 365'te DKIM'i](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)el ile ayarlamak için ne yapmak gerekir?

Genel olarak DNS kayıtlarıyla ilgili yardıma ihtiyacınız varsa, [Office 365 için](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)herhangi bir DNS barındırma hizmet sağlayıcısında DNS kayıtları oluşturma bkz.

> [!NOTE]
> Etki alanınız için DNS barındırma hizmetlerinden DKIM DNS kayıtlarınızı oluşturduktan veya güncelleştirdikten sonra, DNS kayıtlarının yayılmasını beklemeniz gerekir.
