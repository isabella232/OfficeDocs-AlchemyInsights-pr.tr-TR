---
title: Büyük ekler nedeniyle Giden Kutusu'nda sıkışmış
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441325"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Giden Kutusu'nda sıkışmış iletileri düzeltme

[Microsoft Destek ve Kurtarma Yardımcısı](https://diagnostics.office.com/#/) aracından ["E-posta iletileri göndermekte, almakta veya bulmakta sorun yaşıyorum"](https://aka.ms/SaRA-OutlookSendReceive) senaryosunu çalıştırarak başlamanızı öneririz.

Bir ileti Giden Kutunuzda sıkışıp kaldığında, en olası nedenler şunlardır:
- Büyük ekler.
- Bağlı seçenek **etkinleştirilmediğinde hemen Gönder.**

Büyük ekleri kaldırmak için: 

1. Outlook'ta,**İşi Çevrimdışı** **Gönder / Al'ı** > seçin. 
2. Gezinti bölmesinde Giden **Kutusu'nu**seçin. Buradan şunları yapabilirsiniz: 
    - İletiyi silin (seçin ve sonra **Sil'i**seçin).
    - İletiyi Taslaklar klasörünüze sürükleyin, açmak için çift tıklatın ve eki kaldırın seçin ve sonra **Sil'i**seçin).
3. Outlook'un iletiyi iletmeye çalıştığını belirten bir hata alırsanız, Outlook'u kapatın. Çıkmak birkaç dakika sürebilir. Outlook kapanmazsa Ctrl+Alt+Sil tuşuna basın ve **Görev Yöneticisini Başlat'ı**seçin. Görev Yöneticisi'nde, **İşlemler** sekmesini seçin, outlook.exe'ye gidin ve **Son İşlem'i**seçin.
4. Outlook kapandıktan sonra yeniden başlatın ve 2 ve 3 adımlarını yineleyin. 
5. Eki kaldırdıktan sonra, çevrimiçi çalışmaya devam etmek için**İşI Çevrimdışı** **Gönder /Al'ı** > tıklatın. 

İletiler, **Gönder'i**tıklattığınızda giden kutuya da takılıp kalır, ancak bağlı değildir. **Gönder / Al'ı** tıklatın ve **Çevrimdışı İş** düğmesine bakın. Eğer maviyse, bağlantın kesilir. Bağlanmak için seçin (düğme beyaza döner) ve **Tümünü Gönder'e**tıklayın.
 
**Bağlandığında hemen Gönder'i**etkinleştirmek için:
 
- **Dosya** > **Seçenekleri** >  **Gelişmiş'i**seçin.
Gönder **ve al** bölümünde, **bağlandığında hemen Gönder'i**ve ardından **Tamam'ı**seçin.
 
Tüm ayrıntılar için bkz:
- [Video: Sıkışmış bir e-postayı gönderme veya silme](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Outlook'ta el ile bir gönderme/alma işlemi başlatana kadar e-posta Giden Kutusu klasöründe kalır](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
