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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695865"
---
# <a name="fix-transport-rules"></a>Aktarım kurallarını düzeltme

Özel posta akışı kuralı bu iletiyi etkiliyor. Tam kuralı gözden geçirmek için şunları yapın:

1. Gönderme sonuçlarında, Ek bilgilerin altında **GUID** **veya** İlke **Adı'nın notunu yazın.**
2. Exchange Yönetim Kabuğu'nu başlatma. Daha fazla bilgi için [bkz. Exchange Yönetim Kabuğu'nu açma.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Bu komutu çalıştırın (gönderinizin GUID'lerini kullanarak):  **Get-TransportRule -identity "GUID" | fl * Açıklama***
4. İletiyi etkilenen yapılandırılmış koşulları görmek için açıklamayı gözden geçirebilirsiniz.

Daha fazla bilgi edinmek için [Bkz. Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
