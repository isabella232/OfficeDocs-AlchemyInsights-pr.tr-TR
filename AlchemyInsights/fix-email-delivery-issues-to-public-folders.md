---
title: E-posta yla etkin ortak klasörlere e-posta teslim sorunlarını düzeltme
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716372"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>E-posta yla etkin ortak klasörlere e-posta teslim sorunlarını düzeltme

Dış gönderenler posta yla etkinleştirilmiş ortak klasörlerinize ileti gönderemiyorsa ve gönderenler hatayı alıyorsa: **bulunamadı (550 5.4.1)** ortak klasörün e-posta etki alanının yetkili bir etki alanı yerine dahili röle etki alanı olarak yapılandırıldığı doğrula:

1. Exchange [yönetici merkezini (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)açın.

2. Posta **akışına** \> git **Kabul edilen etki alanları,** kabul edilen etki alanını seçin ve sonra **Edit'i**tıklatın.

3. Açılan özellikler sayfasında, etki alanı türü **Yetkili**olarak ayarlanmışsa, değeri **İç röle** olarak değiştirin ve ardından **Kaydet'i**tıklatın.

Harici **gönderenler izniniz yoksa hata alırsanız (550 5.7.13)** ortak klasörde anonim kullanıcıların izinlerini görmek için [Exchange Online PowerShell'de](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) aşağıdaki komutu çalıştırın:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Örneğin, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Harici kullanıcıların bu ortak klasöre e-posta göndermesine izin vermek için CreateItems erişim hakkını Anonim kullanıcıya ekleyin. Örneğin, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
