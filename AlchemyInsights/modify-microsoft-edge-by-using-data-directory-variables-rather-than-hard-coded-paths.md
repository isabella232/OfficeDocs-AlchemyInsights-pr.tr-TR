---
title: Sabit kodlu yollar yerine veri dizini değişkenlerini kullanarak Microsoft Edge'i değiştirme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036860"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Sabit kodlu yollar yerine veri dizini değişkenlerini kullanarak Microsoft Edge'i değiştirme

Örneğin, Windows'da profil verilerini varsayılan konum yerine kullanıcının yerel uygulama verileri altında depolamak *için, UserDataDir* ilkesini **${local_app_data}\Edge\Profile** olarak ayarlayın.

Daha fazla bilgi için [bkz. Microsoft Edge kullanıcı veri dizini değişkenleri oluşturma.](https://docs.microsoft.com/deployedge/microsoft-edge-policies)