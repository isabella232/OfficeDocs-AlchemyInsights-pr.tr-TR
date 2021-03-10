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
# <a name="fix-transport-rules"></a><span data-ttu-id="e50a2-102">Aktarım kurallarını düzeltme</span><span class="sxs-lookup"><span data-stu-id="e50a2-102">Fix transport rules</span></span>

<span data-ttu-id="e50a2-103">Özel posta akışı kuralı bu iletiyi etkiliyor.</span><span class="sxs-lookup"><span data-stu-id="e50a2-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="e50a2-104">Tam kuralı gözden geçirmek için şunları yapın:</span><span class="sxs-lookup"><span data-stu-id="e50a2-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="e50a2-105">Gönderme sonuçlarında, Ek bilgilerin altında **GUID** **veya** İlke **Adı'nın notunu yazın.**</span><span class="sxs-lookup"><span data-stu-id="e50a2-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="e50a2-106">Exchange Yönetim Kabuğu'nu başlatma.</span><span class="sxs-lookup"><span data-stu-id="e50a2-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="e50a2-107">Daha fazla bilgi için [bkz. Exchange Yönetim Kabuğu'nu açma.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="e50a2-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="e50a2-108">Bu komutu çalıştırın (gönderinizin GUID'lerini kullanarak):  **Get-TransportRule -identity "GUID" | fl \* Açıklama**\*</span><span class="sxs-lookup"><span data-stu-id="e50a2-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="e50a2-109">İletiyi etkilenen yapılandırılmış koşulları görmek için açıklamayı gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="e50a2-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="e50a2-110">Daha fazla bilgi edinmek için [Bkz. Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="e50a2-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
