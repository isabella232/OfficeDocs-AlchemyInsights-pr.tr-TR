---
title: Windows'de Bellek Tanılama'yı Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 63ba3afdd8f74b17559484f37e9250587aec9b4a929325d8f82e3c9ad06f1783
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922591"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Windows'de Bellek Tanılama'yı Windows 10

Bilgisayarınız Windows uygulamalar kilitlenmeye, donuyor veya kararsız bir şekilde davranıyorsa, bilgisayarınızın belleğinde (RAM) bir sorun olabilir. Bilgisayarınızın RAM'Windows sorunları kontrol etmek için Bellek Tanılama aracında çalıştırabilirsiniz.

Görev çubuğunuzda arama kutusuna bellek tanılama **yazın ve bellek** tanılamayı Windows **seçin.** 

Tanılamayı çalıştırmak için bilgisayarın yeniden başlatılması gerekiyor. Hemen yeniden başlatma seçeneğiniz vardır (lütfen çalışmanızı kaydedin ve önce açık belgeleri ve e-postaları kapatın) veya bilgisayarı bir sonraki yeniden başlatma işlemi sırasında tanılamanın otomatik olarak çalışacak şekilde zamanlamayı deneyin:

![Windows Bellek Tanılama](media/windows-memory-diagnostic.png)

Bilgisayar yeniden başlatıldığında, Windows **Tanılama Aracı otomatik** olarak çalışır. Tanılamalar çalıştırılıyorken durum ve ilerleme durumu görüntülenir ve klavyenizde **ESC** tuşuna basarak tanılamayı iptal seçeneğiniz vardır.

Tanılama tamamlandığında, Windows başlayacaktır.
Yeniden başlatmanın hemen ardından Masaüstü görüntülendiğinde, herhangi  bir bellek hatası bulunıp buluna olmadığını göstermek için bir bildirim (görev çubuğundaki İşlem Merkezi simgesinin yanında) gösterilir. Örneğin:

İşte İşlem Merkezi simgesi: ![İşlem merkezi simgesi](media/action-center-icon.png) 

Ve örnek bir bildirim: ![Bellek hatası yok](media/no-memory-errors.png)

Bildirimi kaçırdıysanız, İşlem Merkezi'yi görüntülemek ve kaydırılabilir  bir bildirim listesi görmek için görev çubuğunda İşlem Merkezi simgesini seçebilirsiniz. 

Ayrıntılı bilgileri gözden geçirmek için, **görev çubuğunuzda** arama kutusuna olayı yazın ve ardından Olay **Görüntüleyicisi'ni seçin.** Olay **Görüntüleyicisi'nin** sol bölmesinde, Günlükler ve Sistem **Windows'> gidin.** Sağ bölmede, Kaynak sütununa bakarak listeyi  aşağı doğru tarayın; Kaynak değeri **MemoryDiagnostics-Results** ile ilgili olayları görene kadar. Bu tür olayları vurgulayın ve listenin altındaki Genel sekmesinin **altındaki** kutuda sonuç bilgilerini görüntüleyin.
