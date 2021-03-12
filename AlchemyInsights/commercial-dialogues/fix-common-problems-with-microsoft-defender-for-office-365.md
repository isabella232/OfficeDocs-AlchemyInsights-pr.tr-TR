---
title: Office 365 için Microsoft Defender ile ilgili sık karşılaşılan sorunları düzeltme
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
ms.openlocfilehash: 05fa518ece7ea40fd7b4cea57115d9cd60370b01
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750748"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a><span data-ttu-id="f50aa-102">Office 365 için Microsoft Defender ile ilgili sık karşılaşılan sorunları düzeltme</span><span class="sxs-lookup"><span data-stu-id="f50aa-102">Fix common problems with Microsoft Defender for Office 365</span></span>

<span data-ttu-id="f50aa-103">Office 365 için Microsoft Defender ile ilgili sık karşılaşılan sorunların bazı çözümleri:</span><span class="sxs-lookup"><span data-stu-id="f50aa-103">Here are some solutions to common problems with Microsoft Defender for Office 365:</span></span>

- <span data-ttu-id="f50aa-104">**İleti gecikmesi:** İleti teslimi geciktirilirken sorun yaşıyorsanız, Güvenli Ekler ilkeniz  içindeki Dinamik Teslim seçeneklerini kullanmak istemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="f50aa-104">**Message delay:** If you're experiencing issues where message delivery is delayed, you'll want to use the **Dynamic Delivery** options within your Safe Attachments policy.</span></span> <span data-ttu-id="f50aa-105">Daha fazla bilgi edinmek için Güvenli [Ekler ilkelerde Dinamik Teslim'e bakın.](https://go.microsoft.com/fwlink/?linkid=2094106)</span><span class="sxs-lookup"><span data-stu-id="f50aa-105">To learn more, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2094106).</span></span>
- <span data-ttu-id="f50aa-106">**Hatalı pozitif veya negatif sonuçları bildirme:** Şu bağlantıyı kullanarak iletiyi Microsoft'a bildirebilirsiniz: [Microsoft Defender Yanıt Portalı.](https://go.microsoft.com/fwlink/?linkid=2092835)</span><span class="sxs-lookup"><span data-stu-id="f50aa-106">**Report false positive or negative results:** Report the message to Microsoft using this link: [Microsoft Defender Response Portal](https://go.microsoft.com/fwlink/?linkid=2092835).</span></span>
- <span data-ttu-id="f50aa-107">**Güvenli Bağlantı korumasını etkinleştir:**</span><span class="sxs-lookup"><span data-stu-id="f50aa-107">**Enable Safe Link protection:**</span></span>
    1. <span data-ttu-id="f50aa-108">[Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)Güvenlik ve Uyumluluk & oturum açma.</span><span class="sxs-lookup"><span data-stu-id="f50aa-108">Sign in to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
    2. <span data-ttu-id="f50aa-109">Threat Management Policy Safe Links **(Tehdit** Yönetimi İlkesi  >    >  **Güvenli Bağlantılar) bağlantısına gidin.**</span><span class="sxs-lookup"><span data-stu-id="f50aa-109">Go to **Threat Management** > **Policy** > **Safe Links.**</span></span>
    3. <span data-ttu-id="f50aa-110">Belirli **alıcılara uygulanacak İlkeler'in** altında, yapılandırılmış ilkeyi açın.</span><span class="sxs-lookup"><span data-stu-id="f50aa-110">Under **Policies that apply to specific recipients**, open the policy configured.</span></span>
    4. <span data-ttu-id="f50aa-111">**Ayarlar'ın** **altında, kuruluş içinde gönderilen iletilere güvenli bağlantıları uygula'ya tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="f50aa-111">Under **Settings**, select **Apply safe links to messages sent within the organization**.</span></span>
