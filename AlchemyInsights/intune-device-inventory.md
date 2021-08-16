---
title: Intune Cihaz Envanteri
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014092"
---
# <a name="intune-device-inventory"></a>Intune Cihaz Envanteri

The Devices blade, intune'da her cihaz temelinde yönetim altındaki cihazlarla ilgili yönetici içgörü sağlar. Gösterilen bilgiler şunları içerir: Donanım, Bulunan uygulamalar, Cihaz Uyumluluğu durumu ve Cihaz Yapılandırması durumu.

Donanım ve bulunan uygulamalar için envanter verileri yedi günlük bir döngüde toplanır. Bildirilen donanım uygulamaları ve belirli öğeler, cihazın işletim sistemine ve cihazın kişisel ya da kurumsal sahip olup olmadığına bağlı olarak farklılık gösterir.

Daha fazla bilgi için [bkz. Intune'da cihaz ayrıntılarına bakın.](https://docs.microsoft.com/intune/device-inventory)

**SSS**

S: Intune'a kayıtlı ve diğer cihazlarda mevcut uygulamaların tam envanter listesini Windows alam. Neden olmasın?

Y: Şu anda, şirket cihazları olarak tanımlanan Windows 10 bilgisayarlar için yalnızca modern uygulamalar listelenmiştir. Intune, bu cihazlarda yüklü Win32 uygulamaları hakkında bilgi toplamaz.

S: Telefon numaraları neden tüm cihazlardan toplanmaz?

A: Intune'da şirket cihazları olarak kategorilere ayrılmış telefonlar, örneğin bir mobil cihaz envanter raporu çalıştıracaksanız, tam telefon numarasıyla tanımlanmaz. Kendi cihaza ait telefon numaraları her zaman yıldız işaretleriyle (****) kısmen maskelenmiş olur ve yalnızca son dört rakam gösterir.