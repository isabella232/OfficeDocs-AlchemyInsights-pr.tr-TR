---
title: Bağlantı ilkesi düzeltme
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695891"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="299c8-102">Bağlantı ilkesi düzeltme</span><span class="sxs-lookup"><span data-stu-id="299c8-102">Fix connection policy</span></span>

<span data-ttu-id="299c8-103">E-posta güvenli olarak işaretlendi ve gönderen IP adresi Bağlantı Filtresi ilkesinde güvenli olarak işaretlenmiş olduğundan kullanıcının gelen kutusuna teslim edildi.</span><span class="sxs-lookup"><span data-stu-id="299c8-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="299c8-104">İlkeyi gözden geçirmek için şunları yapın:</span><span class="sxs-lookup"><span data-stu-id="299c8-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="299c8-105">[Office 365 Güvenlik ve Uyumluluk &'ne](https://go.microsoft.com/fwlink/p/?linkid=2077143)gidin ve ardından Tehdit yönetimi İlkesi İstenmeyen Postayla   >    >  [Mücadele'ye gidin.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="299c8-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="299c8-106">Özel sekmesinde **Bağlantı** filtresi ilkesi seçin **ve sonra da** İlkeyi **düzenle'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="299c8-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="299c8-107">IP **İzinleri listesini gözden** geçirme.</span><span class="sxs-lookup"><span data-stu-id="299c8-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="299c8-108">Güvenli listenin **etkinleştirildiğinden** emin olun.</span><span class="sxs-lookup"><span data-stu-id="299c8-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="299c8-109">Microsoft, üçüncü taraf güvenilir gönderenlerin kaynaklarına abone olur.</span><span class="sxs-lookup"><span data-stu-id="299c8-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="299c8-110">Güvenli **liste etkinleştirilirse,** bu güvenilir gönderenler yanlışlıkla istenmeyen posta olarak işaretlenir.</span><span class="sxs-lookup"><span data-stu-id="299c8-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="299c8-111">Bu seçeneğin kullanılması, size gelen hatalı pozitif (istenmeyen posta olarak sınıflandırılmış iyi posta) sayısını azaltacak olması nedeniyle bu seçeneğin kullanılması önerilir.</span><span class="sxs-lookup"><span data-stu-id="299c8-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
