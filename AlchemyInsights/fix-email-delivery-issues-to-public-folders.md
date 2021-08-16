---
title: Posta özelliği etkin ortak klasörlere e-posta teslim sorunlarını düzeltme
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
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068832"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Posta özelliği etkin ortak klasörlere e-posta teslim sorunlarını düzeltme

Dış gönderenler posta özellikli ortak klasörlerinize ileti gönderemediyse ve gönderenler şu hatayı alır: bulunamadı **(550 5.4.1)**, ortak klasörün e-posta etki alanının yetkili bir etki alanı yerine iç geçiş etki alanı olarak yapılandırıldığından emin olun:

1. yönetim [Exchange (EAC) açın.](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Posta akışı **Kabul edilen etki** \> **alanları'ne** gidin, kabul edilen etki alanını seçin ve sonra da Düzenle'ye **tıklayın.**

3. Açılan özellikler sayfasında, etki alanı türü Yetkili olarak ayarlanmışsa, değeri  İç geçiş olarak değiştirin ve Kaydet'e **tıklayın.**

Dış gönderenler izniniz yoksa **(550 5.7.13)** hatasını alırsa, ortak klasördeki anonim kullanıcıların izinlerini görmek için [Exchange Online PowerShell'de](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) aşağıdaki komutu çalıştırın:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Örneğin, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Dış kullanıcıların bu ortak klasöre e-posta göndermesine izin vermek için CreateItems erişimini doğrudan kullanıcı Anonim klasörüne ekleyin. Örneğin, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
