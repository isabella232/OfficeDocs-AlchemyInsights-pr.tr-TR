---
title: Etkin posta ortak klasörlere e-posta teslim sorunları düzeltme
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e24a4db2deb3f691209a1634d932ed277a79c868
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387725"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Etkin posta ortak klasörlere e-posta teslim sorunları düzeltme

Dış Gönderenler, etkin posta ortak klasörlere ileti gönderemiyor ve Gönderenler hata iletisini alıyorsunuz: **(550 5.4.1) bulunamadığını belirten**, ortak klasör yerine bir iç aktarma etki alanı olarak yapılandırıldığı için e-posta etki alanını doğrulayın bir yetkili etki alanı:

1. [Exchange Yönetim Merkezi (TZT)](https://docs.microsoft.com/Exchange/exchange-admin-center)açın.

2. **Posta akışı** Git \> **kabul edilen etki alanları**, kabul edilen etki alanını seçin ve sonra **Düzenle**' yi tıklatın.

3. Özellikler için **yetkili**etki alanı türü ayarlanmışsa, bu açılır sayfa, **iç geçiş** için değerini değiştirin ve **Kaydet**' i tıklatın.

Dış Gönderenler hata **(550 5.7.13) izniniz yoksa**alırsanız, [Çevrimiçi PowerShell Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) ortak klasör içinde anonim kullanıcılar için izinleri görmek için aşağıdaki komutu çalıştırın:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Örneğin, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Bu ortak klasöre e-posta göndermek dış kullanıcılara izin vermek için CreateItems erişim hakkı kullanıcı anonim ekleyin. Örneğin, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
