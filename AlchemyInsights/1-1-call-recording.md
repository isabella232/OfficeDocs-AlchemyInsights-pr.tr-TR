---
title: Bire bir arama kaydı
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702110"
---
# <a name="11-call-recording"></a><span data-ttu-id="87669-102">Bire bir arama kaydı</span><span class="sxs-lookup"><span data-stu-id="87669-102">1:1 call recording</span></span>

<span data-ttu-id="87669-103">Bir **aramada** Kaydı Başlat düğmesi gri görüntüye sahipse, etkiyi alan kullanıcının ilke ayarlarını değiştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="87669-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="87669-104">İlke ayarını kontrol etmek için, yukarıdaki **Diag: 1:1** Arama Kaydı yazın ve etki Teams Tanılama'yı çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="87669-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="87669-105">31 Mayıs 2021'den başlayarak, *AllowCloudRecordingForCalls* için yeni bir Çağrı Teams zorlamaya başlayacağız.</span><span class="sxs-lookup"><span data-stu-id="87669-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="87669-106">Bu değişiklikten önce, 1:1 arama kaydı Toplantı İlkesi'ne göre *AllowCloudRecording* Teams denetlenir.</span><span class="sxs-lookup"><span data-stu-id="87669-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="87669-107">Bu değişiklik İleti Merkezi gönderisinde belgelenmektedir: [(Güncelleştirildi) 1:1 Arama kaydı ilkesi giriş.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)</span><span class="sxs-lookup"><span data-stu-id="87669-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="87669-108">*AllowCloudRecordingForCalls*   arama ilkesi seçeneği varsayılan olarak **$False** olarak ayarlanır.</span><span class="sxs-lookup"><span data-stu-id="87669-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="87669-109">Tüm kullanıcıların bire bir arama kaydetmelerini engellemeyi tercih ederseniz herhangi bir işleme gerek yok.</span><span class="sxs-lookup"><span data-stu-id="87669-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="87669-110">Bire bir aramalarda tüm kullanıcılarda arama kaydını etkinleştirmek için [Teams PowerShell](/microsoftteams/teams-powershell-install) kullanarak aşağıdaki cmdlet'i çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="87669-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="87669-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="87669-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="87669-112">Alternatif olarak, yeni bir ilke oluşturabilir ve **-AllowCloudRecordingForCalls** $true bu ilkeyi ayarlayarak kullanıcılarınıza atabilirsiniz. </span><span class="sxs-lookup"><span data-stu-id="87669-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="87669-113">Daha fazla bilgi için [bkz. 1:1 Arama Kaydı İlkesi Denetimleri (Neredeyse!) Burada.](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)</span><span class="sxs-lookup"><span data-stu-id="87669-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
