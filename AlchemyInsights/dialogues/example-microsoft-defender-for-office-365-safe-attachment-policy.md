---
title: Office 365 için Microsoft Defender Güvenli Ek ilkesi örneği
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695189"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="90aae-102">Office 365 için Microsoft Defender Güvenli Ek ilkesi örneği</span><span class="sxs-lookup"><span data-stu-id="90aae-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="90aae-103">Bu ayarlar, iletileri hemen teslim edecek *ve* sonra taranan ekleri yeniden eklerken gecikme yok adlı bir ilkeyi etkinleştirir:</span><span class="sxs-lookup"><span data-stu-id="90aae-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="90aae-104">**Ad**: Gecikme yok</span><span class="sxs-lookup"><span data-stu-id="90aae-104">**Name**: No delays</span></span>
- <span data-ttu-id="90aae-105">**Açıklama**: İletileri anında teslim edin ve taratktan sonra ekleri yeniden iliştirin.</span><span class="sxs-lookup"><span data-stu-id="90aae-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="90aae-106">**Yanıt:** Dinamik Teslim **seçeneğini** belirtin.</span><span class="sxs-lookup"><span data-stu-id="90aae-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="90aae-107">Daha fazla bilgi için, Güvenli [Ekler ilkelerde Dinamik Teslim'e bakın.](https://go.microsoft.com/fwlink/?linkid=2092328)</span><span class="sxs-lookup"><span data-stu-id="90aae-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="90aae-108">**Eki yeniden** yönlendirme bölümü: Yeniden yönlendirmeyi etkinleştir seçeneğini belirtin ve ardından kötü amaçlı ekleri araştıracak Microsoft 365 genel yöneticinizin, güvenlik yöneticinizin veya güvenlik analistinizin e-posta adresini girin.</span><span class="sxs-lookup"><span data-stu-id="90aae-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="90aae-109">**Uygulanan bölüm:** Alıcı **etki alanını seçin ve** sonra da etki alanınızı seçin.</span><span class="sxs-lookup"><span data-stu-id="90aae-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="90aae-110">**Ekle'yi** ve ardından Tamam'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="90aae-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="90aae-111">Bitirdikten sonra Kaydet'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="90aae-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="90aae-112">Daha fazla bilgi edinmek için [Office 365 için Microsoft Defender'daki Güvenli Ekler'e bakın.](https://go.microsoft.com/fwlink/?linkid=2092213)</span><span class="sxs-lookup"><span data-stu-id="90aae-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
