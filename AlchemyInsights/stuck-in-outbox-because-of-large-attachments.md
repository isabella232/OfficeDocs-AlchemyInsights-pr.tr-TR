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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232650"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Giden Kutusu'nda sıkışmış iletileri düzeltme

Etkilenen makinedeki [Microsoft Destek ve Kurtarma Yardımcısı](https://diagnostics.office.com/#/) aracından ["E-posta iletileri göndermekte, almakta veya bulmakta sorun yaşıyorum"](https://aka.ms/SaRA-OutlookSendReceive) senaryosunu çalıştırarak başlamanızı öneririz.

Giden Kutunuzda bir ileti sıkışıp kaldığında, bunun en olası nedeni büyük bir ek veya "Bağlandığında hemen gönder" seçeneği etkin değildir.

**Büyük eki kaldırma**

1. **İşi Çevrimdışı** **Gönder / Al'ı** > tıklatın. 
2. Gezinti **bölmesinde, Giden Kutusu'nu**tıklatın. Buradan şunları yapabilirsiniz: 
    - İletiyi silin. Sadece seçin ve **Sil'e**tıklayın.
    - İletiyi **taslaklar klasörünüze**sürükleyin, iletiyi açmak için çift tıklatın ve eki silin (tıklatın ve **Sil'i**tıklatın).
3. Bir hata size Outlook'un iletiyi iletmeye çalıştığını söylüyorsa, Outlook'u kapatın. Çıkmak birkaç dakika sürebilir. Outlook kapanmazsa **Ctrl+Alt+Sil** tuşuna basın ve **Görev Yöneticisini Başlat'ı**tıklatın. Görev Yöneticisi'nde, **İşlemler** sekmesini seçin, outlook.exe'ye gidin ve **Son İşlem'i**tıklatın.
4. Outlook kapandıktan sonra Outlook'u yeniden başlatın ve 2-3 adımlarını yineleyin. 
5. Eki kaldırdıktan sonra, düğmeyi seçmek ve çevrimiçi çalışmaya devam etmek için **Çevrimdışı Gönder /Al'ı** > **Work Offline** tıklatın. 

İletiler, **Gönder'i**tıklattığınızda giden kutuya da takılıp kalır, ancak bağlı değildir. **Gönder / Al'ı** tıklatın ve **Çevrimdışı İş** düğmesine bakın. Eğer maviyse, bağlantın kesilir. Bağlanmak için tıklatın (düğme beyaza döner) ve **Tümünü Gönder'e**tıklayın.
 
**Bağlıyken hemen Gönder'i etkinleştirin**
 
1. Dosya sekmesinde **Seçenekler'i**tıklatın.

2. Outlook Seçenekleri iletişim kutusunda **Gelişmiş'i**tıklatın.

3. Gönder ve al bölümünde, **bağlandığında hemen Gönder'i**etkinleştirmek için tıklatın. **Tamam**'a tıklayın.
 
Tüm ayrıntılar için bkz:
- [Video: Sıkışmış bir e-postayı gönderme veya silme](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Outlook'ta el ile bir gönderme/alma işlemi başlatana kadar e-posta Giden Kutusu klasöründe kalır](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
