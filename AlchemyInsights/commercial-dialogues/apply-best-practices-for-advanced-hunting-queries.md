---
title: Gelişmiş arama sorguları için en iyi yöntemleri uygulama
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930153"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Gelişmiş arama sorguları için en iyi yöntemleri uygulama

Sonuçları daha hızlı elde etmek ve karmaşık sorguları çalıştırırken zaman aşımını önlemek için, şu en iyi yöntemleri uygulayabilirsiniz:

- Aşırı büyük sonuç kümeleri almaktan kaçınmak için, yeni sorguları çalışırken her zaman bir sınır kullanın. Ayrıca, `count` sonuç kümesi boyutunun ilk değerlendirmesini yapmak için kullanın.
- Önce zaman filtrelerini kullanın. İdeal olan, sorgularınızı yedi günle sınırlandırmadır.
- Sorgunun başında, zaman filtresinin hemen ardından, verilerin büyük bir çoğunun kaldır olması gereken filtreleri ekleyin.
- Tam belirteçleri arıyorken, yerine `has` işleci `contains` kullanın.
- Tüm sütunlar yerine belirli bir sütunda arama çalıştırın.
- Tabloları katılırken, önce tabloyu daha az satırla belirtin.
- `project` yalnızca katıldığım tablolardan gerekli sütunlar.

Daha fazla bilgi edinmek için [bkz. Gelişmiş arama sorgusu en iyi yöntemleri.](https://go.microsoft.com/fwlink/?linkid=2144812)
