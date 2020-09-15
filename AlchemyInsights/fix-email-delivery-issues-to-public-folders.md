---
title: Posta etkin ortak klasörler için e-posta teslim sorunlarını düzeltme
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677948"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Posta etkin ortak klasörler için e-posta teslim sorunlarını düzeltme

Dış Gönderenler posta özellikli ortak klasörlerinize ileti gönderemediğinde ve Gönderenler hatayı alıyorsa: **bulunamadı (550 5.4.1)**, ortak klasörün e-posta etki alanının yetkili etki alanı yerine iç geçiş etki alanı olarak yapılandırıldığını doğrulayın:

1. [Exchange Yönetim merkezini (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)açın.

2. **Posta akışı** \> **kabul edilen etki alanlarına**gidin, kabul edilen etki alanını seçin ve **Düzenle**'ye tıklayın.

3. Açılan Özellikler sayfasında, etki alanı türü **yetkili**olarak ayarlanmışsa, değeri **iç geçiş** olarak değiştirin ve **Kaydet**'e tıklayın.

Dış Gönderenler **izniniz olmayan (550 5.7.13)** bir hatayı alıyorsa, ortak klasördeki anonim kullanıcıların izinlerini görmek Için [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) 'de aşağıdaki komutu çalıştırırsınız:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Örneğin, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Dış kullanıcıların bu ortak klasöre e-posta göndermesine izin vermek için anonim öğeleri Access 'e anonim olarak ekleyin. Örneğin, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
