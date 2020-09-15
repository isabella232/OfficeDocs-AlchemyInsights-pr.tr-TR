---
title: 'Hata: Bu bilgisayardaki kurallar uyuşmuyor'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690983"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Hata: Bu bilgisayardaki kurallar uyuşmuyor

Bu bilinen sorunun güncelleştirilmiş durumunu görmek için, [Bu bilgisayardaki kuralların Microsoft Exchange 'deki kurallarla eşleşmediğini](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) görün

Outlook ekibi, derleme 12928,10000 ' te bir düzeltme uygulamıştır. Düzeltme zaten Insider 'dan hızlıdır ve 2020 Haziran 'da aylık kanala gider. Sabit yapıya sahip olduktan sonra "hangi kuralları korumak istiyorsunuz" istemini son kez alabilirsiniz. İstendiğinde sunucu 'yu seçin ve ardından Outlook 'a geri dönün ve devre dışı bırakılmış kuralları yeniden etkinleştirin.

Düzeltme mevcut olana kadar aşağıdaki geçici çözümü kullanın:

**Geçici çözüm**: son raporlarda, sorun yalnızca Outlook masaüstü 'nde istemci kuralları oluşturmuş olanlar için ortaya çıktı. Sorun devam ederseniz, kuralları silin ve sonra sorun giderilinceye kadar yalnızca OWA (Outlook Web App) kurallarını oluşturup düzenleyin.

Kuralları el ile silemsem Outlook 'U başlattığınızda Outlook.exe/cleankurallarını çalıştırarak Outlook komutunu çalıştırabilirsiniz. Bu, hem istemci hem de sunucu kurallarını silecek. Outlook profilindeki tüm hesapların tüm kurallarını silecek. Bu komut, komut satırı anahtarları makalesinde daha da belgelenmiştir.

