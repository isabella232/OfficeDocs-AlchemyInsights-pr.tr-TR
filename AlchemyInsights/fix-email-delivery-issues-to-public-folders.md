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
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366484"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Posta etkin ortak klasörler için e-posta teslim sorunlarını düzeltme

Dış Gönderenler posta özellikli ortak klasörlerinize ileti gönderemediğinde ve Gönderenler hatayı alıyorsa: **bulunamadı (550 5.4.1)**, ortak klasörün e-posta etki alanının yetkili etki alanı yerine iç geçiş etki alanı olarak yapılandırıldığını doğrulayın:

1. [Exchange Yönetim merkezini (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)açın.

2. **Posta akışı** \> **kabul edilen etki alanlarına**gidin, kabul edilen etki alanını seçin ve **Düzenle**'ye tıklayın.

3. Açılan Özellikler sayfasında, etki alanı türü **yetkili**olarak ayarlanmışsa, değeri **iç geçiş** olarak değiştirin ve **Kaydet**'e tıklayın.

Dış Gönderenler **izniniz olmayan (550 5.7.13)** bir hatayı alıyorsa, ortak klasördeki anonim kullanıcıların izinlerini görmek Için [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) 'de aşağıdaki komutu çalıştırırsınız:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Örneğin, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Dış kullanıcıların bu ortak klasöre e-posta göndermesine izin vermek için anonim öğeleri Access 'e anonim olarak ekleyin. Örneğin, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
