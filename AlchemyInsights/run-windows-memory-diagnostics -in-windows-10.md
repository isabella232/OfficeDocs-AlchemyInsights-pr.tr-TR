---
title: Windows 10'da Windows Bellek Tanılama'yı çalıştırma
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
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826687"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Windows 10'da Windows Bellek Tanılama'yı çalıştırma

Bilgisayarınızda Windows ve uygulamalar kilitlenmeye, donuyorsa veya kararsız bir şekilde davranıyorsa, bilgisayarınızın belleğinde (RAM) bir sorun olabilir. Bilgisayarınızın RAM'iyle ilgili sorunları kontrol etmek için Windows Bellek Tanılama'yı çalıştırabilirsiniz.

Görev çubuğunuzda arama kutusuna bellek tanılama **yazın ve** ardından Windows Bellek **Tanılama'yı seçin.** 

Tanılamayı çalıştırmak için bilgisayarın yeniden başlatılması gerekiyor. Hemen yeniden başlatma seçeneğiniz vardır (lütfen çalışmanızı kaydedin ve önce açık belgeleri ve e-postaları kapatın) veya bilgisayarı bir sonraki yeniden başlatma işlemi sırasında tanılamanın otomatik olarak çalışacak şekilde zamanlamayı deneyin:

![Windows Hafıza Tanılama](media/windows-memory-diagnostic.png)

Bilgisayar yeniden başlatıldığında Windows Bellek **Tanılama Aracı otomatik** olarak çalışır. Tanılamalar çalıştırılıyorken durum ve ilerleme durumu görüntülenir ve klavyenizde **ESC** tuşuna basarak tanılamayı iptal seçeneğiniz vardır.

Tanılama tamamlandığında, Windows normal şekilde başlar.
Yeniden başlatmanın hemen ardından Masaüstü görüntülendiğinde, herhangi  bir bellek hatası bulunıp buluna olmadığını göstermek için bir bildirim (görev çubuğundaki İşlem Merkezi simgesinin yanında) gösterilir. Örneğin:

İşte İşlem Merkezi simgesi: ![İşlem merkezi simgesi](media/action-center-icon.png) 

Ve örnek bir bildirim: ![Bellek hatası yok](media/no-memory-errors.png)

Bildirimi kaçırdıysanız, İşlem Merkezi'yi görüntülemek ve kaydırılabilir  bir bildirim listesi görmek için görev çubuğunda İşlem Merkezi simgesini seçebilirsiniz. 

Ayrıntılı bilgileri gözden geçirmek için, **görev çubuğunuzda** arama kutusuna olayı yazın ve ardından Olay **Görüntüleyicisi'ni seçin.** Olay **Görüntüleyicisi'nin** sol bölmesinde, Windows Günlükleri ve **Sistem > gidin.** Sağ bölmede, Kaynak sütununa bakarak listeyi  aşağı doğru tarayın; Kaynak değeri **MemoryDiagnostics-Results** ile ilgili olayları görene kadar. Bu tür olayları vurgulayın ve listenin altındaki Genel sekmesinin **altındaki** kutuda sonuç bilgilerini görüntüleyin.
