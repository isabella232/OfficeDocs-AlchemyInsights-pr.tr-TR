---
title: Microsoft Defender Gelişmiş Tehdit Koruması'nda (ATP) Windows dışı cihazlarla birlikte çıkar
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748486"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="7d425-102">Microsoft Defender Gelişmiş Tehdit Koruması'nın (ATP) Windows dışı cihazlardan çıkarı</span><span class="sxs-lookup"><span data-stu-id="7d425-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="7d425-103">Bunu şu şekilde yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="7d425-103">Here's how:</span></span>

1. <span data-ttu-id="7d425-104">Üçüncü taraf çözümünün Microsoft Defender ATP ile bağlantısını kesmek için üçüncü taraf belgelerini izleyin.</span><span class="sxs-lookup"><span data-stu-id="7d425-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="7d425-105">Azure Active Directory kiracınıza, üçüncü taraf çözümünün izinlerini kaldırın:</span><span class="sxs-lookup"><span data-stu-id="7d425-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="7d425-106">[Azure portalında oturum açın.](https://go.microsoft.com/fwlink/?linkid=2125612)</span><span class="sxs-lookup"><span data-stu-id="7d425-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="7d425-107">Azure Active Directory **Kurumsal**  >  **Uygulamaları'nın Tüm** hizmetlerini  >  **seçin.**</span><span class="sxs-lookup"><span data-stu-id="7d425-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="7d425-108">Kullanmak istediğiniz uygulamayı seçin.</span><span class="sxs-lookup"><span data-stu-id="7d425-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="7d425-109">**Sil'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="7d425-109">Select **Delete**.</span></span>

<span data-ttu-id="7d425-110">Daha fazla bilgi edinmek için [Windows dışı cihazlara bakın.](https://go.microsoft.com/fwlink/?linkid=2143630)</span><span class="sxs-lookup"><span data-stu-id="7d425-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
