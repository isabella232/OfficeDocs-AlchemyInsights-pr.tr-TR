---
title: SharePoint ve OneDrive uyarılarını alırken gecikmeler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 92e517ae6e83aa91b9838047ec77759dc893bc57
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/17/2020
ms.locfileid: "46785685"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="07aba-102">SharePoint ve OneDrive uyarılarını alırken gecikmeler</span><span class="sxs-lookup"><span data-stu-id="07aba-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="07aba-103">İlk olarak, e-postanızın önemsiz veya Istenmeyen klasörünü denetleyin.</span><span class="sxs-lookup"><span data-stu-id="07aba-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="07aba-104">**Birden çok dosya veya kitaplıklardaki tüm uyarılar gecikirse**, [hizmet durumu panosunu](https://portal.office.com/adminportal/home?ref=/servicehealth) ziyaret ederek SharePoint veya Exchange 'le ilgili tüm Danışma belgelerini/olaylarını denetleyin.</span><span class="sxs-lookup"><span data-stu-id="07aba-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="07aba-105">Sorun SharePoint uyarısı yeteneği veya Exchange aracılığıyla e-postalarda gecikmelere neden olabilir.</span><span class="sxs-lookup"><span data-stu-id="07aba-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="07aba-106">Ayrıca, diğer e-postanın teslim edilip edilmediğini de unutmayın, sorun büyük olasılıkla Exchange gecikmelerinden kaynaklanıyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="07aba-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="07aba-107">**Belirli bir dosya veya kitaplıktan gelen bir uyarı teslim edilmediyse**, silmeyi ve yeniden oluşturmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="07aba-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="07aba-108">Uyarıyı yeniden oluşturmak için [SharePoint uyarılarını yönetme, görüntüleme veya silme](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="07aba-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="07aba-109">Bir dağıtım grubuna uyarı gönderilemez.</span><span class="sxs-lookup"><span data-stu-id="07aba-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="07aba-110">Yalnızca güvenlik ve O365 grupları desteklenir.</span><span class="sxs-lookup"><span data-stu-id="07aba-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="07aba-111">Uyarı e-posta şablonlarını özelleştiremezsiniz.</span><span class="sxs-lookup"><span data-stu-id="07aba-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="07aba-112">Bunları başarmak için Microsoft Flow veya SharePoint Designer Iş akışını kullanmalısınız.</span><span class="sxs-lookup"><span data-stu-id="07aba-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
