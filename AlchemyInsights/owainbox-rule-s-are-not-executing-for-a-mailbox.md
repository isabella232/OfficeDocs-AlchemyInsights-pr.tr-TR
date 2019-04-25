---
title: 1332 - OWA gelen kutusu kuralları bir posta kutusu için yürütülen değil
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372580"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Gelen kutusu kuralı beklendiği gibi çalışmıyor

Aşağıdaki ayarları doğrulayın:

- Bir ileti, iletilen veya yanıtlanan dayanarak otomatik olarak gelen kutusu kuralları üzerinde yalnızca bir kez yeniden yönlendirilebilir. Bir yeniden yönlendirme kuralı (bir gelen kutusu kuralı veya posta akışı kuralı, bir aktarım kuralı olarak da bilinir) en çok on iletme alıcıların iletiye ekleyebilirsiniz. [Günlük, taşıma ve gelen kutusu kuralı sınırlarını](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)daha fazla bilgi için bkz.

- Gelen Kutusu kuralları diğer günlük kaydı posta kutusunun üzerinde çalışmaz. [Diğer günlük kaydı posta kutusu](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)posta kutusu diğer günlük kaydı hakkında daha fazla bilgi için bkz.

Bu sorunları gidermek için bkz: [KB 2829319](https://support.microsoft.com/kb/2829319).

Yukarıdaki sorunlar uygulamazsanız, Microsoft Support sorunu üst düzeye iletmeden önce gelen kutusu kuralı Tanılama raporunu çalıştırın:

1. Web'de Outlook'taki posta kutusunu açın ve **Ayarlar** ' ı tıklatın \> **seçenekleri** \> **Düzenle e-posta** \> **Gelen Kutusu kuralları**.

2. Sayfanın alt kısmında, **kurallarınızın bir tanılama raporu oluşturmak için burayı tıklatın çalışıyorsanız değil'i**tıklatın.
