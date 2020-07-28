---
title: Takımlar özel kanalSilme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439911"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="488f1-102">Takımlar özel kanalSilme</span><span class="sxs-lookup"><span data-stu-id="488f1-102">Delete a Teams private channel</span></span>

<span data-ttu-id="488f1-103">Microsoft, altta yatan SharePoint sitesi için SharePoint Bekletme İlkeleri etkinleştirilmişse, Takımlar özel kanalısilme sorununun farkındadır.</span><span class="sxs-lookup"><span data-stu-id="488f1-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="488f1-104">Microsoft bir düzeltme üzerinde çalışıyor.</span><span class="sxs-lookup"><span data-stu-id="488f1-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="488f1-105">Bu arada, özel kanalı silmek için aşağıdaki geçici geçici çözümlerini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="488f1-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="488f1-106">**Takım/site koleksiyonunu Sharepoint bekletme ilkesinden hariç tinleyin.**</span><span class="sxs-lookup"><span data-stu-id="488f1-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="488f1-107">Office 365 yönetici portalına gidin ve sol daki gezinti bölmesinde **tümünü göster'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="488f1-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="488f1-108">**Yönetici merkezleri**altında, Güvenlik **& Uyumluluk**Veri Kaybı  >  **Önleme**  >  **Politikası'na**gidin.</span><span class="sxs-lookup"><span data-stu-id="488f1-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="488f1-109">Sharepoint siteleri için geçerli olan herhangi bir ilkeyi belirleyin ve özel kanalı içeren Ekibin Sharepoint sitesinin bekletme ilkesine dahil olmaması için politikayı değiştirin.</span><span class="sxs-lookup"><span data-stu-id="488f1-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="488f1-110">İlkeyi kaydet.</span><span class="sxs-lookup"><span data-stu-id="488f1-110">Save the policy.</span></span>
    <span data-ttu-id="488f1-111">İlke ayarlarının etkili olması 24 saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="488f1-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="488f1-112">Site dışlandıktan sonra, özel kanalı silebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="488f1-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="488f1-113">Android ***might*** cihazınızda Microsoft Ekipleri'ni kullanarak özel kanalı silebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="488f1-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="488f1-114">İlgili SharePoint bilgileri [için](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)bkz.</span><span class="sxs-lookup"><span data-stu-id="488f1-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>