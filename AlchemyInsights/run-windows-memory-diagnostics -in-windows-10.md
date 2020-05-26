---
title: Windows 10'da Windows Bellek Tanılama'yı çalıştırma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358291"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Windows 10'da Windows Bellek Tanılama'yı çalıştırma

Bilgisayarınızdaki Windows ve uygulamalar çöküyorsa, donuyorsa veya kararsız bir şekilde hareket ediyorsa, bilgisayarın belleğinde (RAM) sorun yaşayabilirsiniz. Bilgisayarın RAM'iyle ilgili sorunları denetlemek için Windows Memory Diagnostic'i çalıştırabilirsiniz.

Görev çubuğunuzdaki arama kutusunda **bellek tanılama**yazın ve ardından **Windows Memory Diagnostic'i**seçin. 

Tanılamayı çalıştırmak için bilgisayarın yeniden başlatılması gerekir. Hemen yeniden başlatma seçeneğiniz vardır (lütfen önce çalışmanızı kaydedin ve açık belgeleri ve e-postaları kapatın) veya bilgisayarı bir sonraki kez yeniden başlatında otomatik olarak çalışacak tanılamayı zamanlayın:

![Windows Bellek Tanılama](media/windows-memory-diagnostic.png)

BILGISAYAR yeniden başlatıldığında, **Windows Bellek Tanılama Aracı** otomatik olarak çalışır. Durum ve ilerleme tanılama çalıştırılınrken görüntülenir ve klavyenizdeki **ESC** tuşuna basarak tanılamayı iptal etme seçeneğiniz vardır.

Tanılama tamamlandığında, Windows normal olarak başlar.
Yeniden başlatmadan hemen sonra, Masaüstü göründüğünde, bellek hataları nın bulunup bulunmadığını belirtmek için bir bildirim (görev çubuğundaki **İşlem Merkezi** simgesinin yanında) görüntülenir. Örneğin:

İşte İşlem Merkezi simgesi: ![İşlem merkezi simgesi](media/action-center-icon.png) 

Ve örnek bir bildirim: ![Bellek hatası yok](media/no-memory-errors.png)

Bildirimi kaçırdıysanız, **İşlem Merkezi'ni** görüntülemek ve kaydırılabilir bir bildirim listesini görmek için görev çubuğundaki **İşlem Merkezi** simgesini seçebilirsiniz.

Ayrıntılı bilgileri gözden geçirmek için görev çubuğunuzdaki arama kutusuna **olay** yazın ve ardından **Olay Görüntüleyicisi'ni**seçin. Olay **Görüntüleyicisi'nin**sol bölmesinde, **Windows Günlükleri > Sistemi'ne**gidin. Sağ bölmede, Kaynak değeri **MemoryDiagnostics-Results**olan olayları görene kadar **Kaynak** sütuna bakarken listeyi aşağı tarayın. Bu tür her bir olayı vurgulayın ve listenin altındaki **Genel** sekmesinin altındaki kutuda sonuç bilgilerini görün.
