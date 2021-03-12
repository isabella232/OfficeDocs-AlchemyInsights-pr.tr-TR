---
title: Gelişmiş av sorguları için en iyi yöntemleri uygulama
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
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749552"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Gelişmiş av sorguları için en iyi yöntemleri uygulama

Sonuçları daha hızlı elde etmek ve karmaşık sorguları çalıştırırken zaman aşımından kaçınmak için, şu en iyi yöntemleri uygulayabilirsiniz:

- Yeni sorguları deniyorum, aşırı büyük sonuç kümelerini almaktan kaçınmak için her zaman bir sınır kullanın. Ayrıca, `count` sonuç kümesi boyutunun ilk değerlendirmesini yapmak için de kullanın.
- Önce zaman filtrelerini kullanın. İdeal olan, sorgularınızı yedi günle sınırlandırma.
- Sorgunun en başında, zaman filtresinin hemen ardından, verilerin büyük bir çoğunun kaldır olması beklenen filtreleri ekleyin.
- Tam belirteçleri arıyorken, bunun yerine `has` işleci `contains` kullanın.
- Tüm sütunlar yerine belirli bir sütunda arama çalıştırın.
- Tabloları katılırken, önce tabloyu daha az satırla belirtin.
- `project` yalnızca katıldığım tablolardan gerekli sütunlar.

Daha fazla bilgi edinmek için gelişmiş [av sorgusu en iyi yöntemlerine bakın.](https://go.microsoft.com/fwlink/?linkid=2144812)
