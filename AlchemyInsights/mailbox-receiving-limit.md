---
title: Sınır zorlaması alan posta kutusu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/31/2021
ms.locfileid: "59316284"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Sınır zorlaması alan posta kutusu

Microsoft yakın zamanda, saatte 3600 ileti için posta kutusu başına eşiği zorlamaya başladı. Daha fazla bilgi için [bkz. Exchange Online.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits) Microsoft 365 içinde 3600'den fazla ileti alan posta kutuları, sonraki 60 dakika boyunca kısıtlandı. 

Buna ek olarak, bir posta kutusunun belirli bir gönderenden aldığı iletileri engelleyen gönderen Microsoft 365 çiftleri (RP) sınırı uygulanır. Tek bir gönderen, toplam eşiğin %33'ü veya iş başına 1200 iletiyi belirli bir alıcıya gönderirse,RP sınırı geçerli olur ve posta kutusu artık söz konusu gönderenden gelen iletileri kabul etmez. Unutmayın:

- Bu sınır, diğer kiracılardan, şirket içi veya İnternet gönderenlerinden alınan e-postalara yönelik bir uygulamadır.
- E-postanın posta kutusuna teslimi önümüzdeki 60 dakika engellenir. 
- Bu posta kutularına gönderenler, posta kutusunun en yüksek teslim eşiğini aşmış olduğunu belirten bir teslim dışı rapor (5.2.121 veya 5.2.122) alır. Kiracılar (aynı kiracı içindeki posta) teslim edilir.
- RP sınırı uygulandığında, alıcı posta kutusu diğer gönderenlerden gelen iletileri kabul etmeye devam eder.

Yöneticiler, "Posta kutuları alma sınırlarını aşıyor" adlı yönetim merkezinde yeni bir rapora Exchange içgörüye erişerek geçerli posta kutusu etkinliğini izleyebilir. Bu içgörü ancak bir kiracı posta kutularını kırıyorsa ve rapor her zaman panoda görünür, ancak kiracı posta kutularını sorun değilse boşsa görüntülenir.

Bilgi alma sınırları hakkında daha fazla bilgi için, yeni EAC'de posta kutuları hakkında bilgi almayı aşan [posta kutularına bakın.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Alma sınırlarının aşıldı raporu hakkında daha fazla bilgi için bkz. Yeni [EAC'de](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)posta kutuları alma sınırları raporunu aşar.