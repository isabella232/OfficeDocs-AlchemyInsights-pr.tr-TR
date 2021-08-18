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
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324010"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>DKIM kayıt biçimlendirmesi ile ilgili sık karşılaşılan sorunları düzeltme

DKIM ayarlama sorunlarının çoğu hatalı DNS kayıtlarıyla ilgili.

DKIM ayarlama sorunlarını düzeltmek için DKIM CNAME **kaydının** (TXT kaydı değil) doğru biçimlendirilmiş olduğunu doğrulayın. Daha fazla bilgi için [bkz. DkIM'i](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)el ile ayarlamak için Office 365.

Genel olarak DNS kayıtlarıyla ilgili yardıma ihtiyacınız varsa, bkz. DNS kayıtları için herhangi bir [DNS barındırma Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

**Not:** Etki alanınız için DNS barındırma hizmette DKIM DNS kayıtlarınızı oluşturduktan veya güncelleştirdikten sonra, DNS kayıtlarının yayılmasını beklemeniz gerekir.
