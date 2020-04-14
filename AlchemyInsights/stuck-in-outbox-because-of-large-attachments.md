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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241272"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Giden Kutusu'nda sıkışmış iletileri düzeltme

[Microsoft Destek ve Kurtarma Yardımcısı](https://diagnostics.office.com/#/) aracından ["E-posta iletileri göndermekte, almakta veya bulmakta sorun yaşıyorum"](https://aka.ms/SaRA-OutlookSendReceive) senaryosunu çalıştırarak başlamanızı öneririz.

Giden Kutunuzda bir ileti sıkışıp kaldığında, bunun en olası nedeni büyük bir ek veya "Bağlandığında hemen gönder" seçeneği etkin değildir.

**Büyük eki kaldırma**

1. Outlook'ta,**İşi Çevrimdışı** **Gönder / Al'ı** > seçin. 
2. Gezinti bölmesinde Giden **Kutusu'nu**seçin. Buradan şunları yapabilirsiniz: 
    - İletiyi silin (seçin ve sonra **Sil'i**seçin).
    - İletiyi Taslaklar klasörünüze sürükleyin, açmak için çift tıklatın ve eki kaldırın seçin ve sonra **Sil'i**seçin).
3. Outlook'un iletiyi iletmeye çalıştığını belirten bir hata alırsanız, Outlook'u kapatın. Çıkmak birkaç dakika sürebilir. Outlook kapanmazsa Ctrl+Alt+Sil tuşuna basın ve **Görev Yöneticisini Başlat'ı**seçin. Görev Yöneticisi'nde, **İşlemler** sekmesini seçin, outlook.exe'ye gidin ve **Son İşlem'i**seçin.
4. Outlook kapandıktan sonra yeniden başlatın ve 2 ve 3 adımlarını yineleyin. 
5. Eki kaldırdıktan sonra, çevrimiçi çalışmaya devam etmek için**İşI Çevrimdışı** **Gönder /Al'ı** > tıklatın. 

İletiler, **Gönder'i**tıklattığınızda giden kutuya da takılıp kalır, ancak bağlı değildir. **Gönder / Al'ı** tıklatın ve **Çevrimdışı İş** düğmesine bakın. Eğer maviyse, bağlantın kesilir. Bağlanmak için tıklatın (düğme beyaza döner) ve **Tümünü Gönder'e**tıklayın.
 
**Bağlıyken hemen Gönder'i etkinleştirin**
 
1. Dosya sekmesinde **Seçenekler'i**tıklatın.

2. Outlook Seçenekleri iletişim kutusunda **Gelişmiş'i**tıklatın.

3. Gönder ve al bölümünde, **bağlandığında hemen Gönder'i**etkinleştirmek için tıklatın. **Tamam**'a tıklayın.
 
Tüm ayrıntılar için bkz:
- [Video: Sıkışmış bir e-postayı gönderme veya silme](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Outlook'ta el ile bir gönderme/alma işlemi başlatana kadar e-posta Giden Kutusu klasöründe kalır](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
