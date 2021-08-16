---
title: Aktarım kurallarını düzeltme
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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034774"
---
# <a name="fix-transport-rules"></a>Aktarım kurallarını düzeltme

Özel posta akışı kuralı bu iletiyi etkiliyordi. Tam kuralı gözden geçirmek için şunları yapın:

1. Gönderme sonuçlarında, Ek bilgiler **altında,** GUID'ye veya **İlke** **Adı'ne dikkat edin.**
2. Yönetim Exchange'i başlatma. Daha fazla bilgi için [bkz. Exchange Kabuğu'nu açma.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Bu komutu çalıştırın (gönderinizin GUID'ini kullanarak):  **Get-TransportRule -identity "GUID" | fl * Açıklama***
4. İletiyi etkilenen yapılandırılmış koşulları görmek için açıklamayı gözden geçirme.

Daha fazla bilgi edinmek için [bkz. Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
