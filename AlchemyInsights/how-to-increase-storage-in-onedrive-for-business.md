---
title: OneDrive Iş 'te depolamayı arttırma
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 676b17d47ee5071ed45e8d6022eaa82b51fc4d51
ms.sourcegitcommit: ad2d185aa9e08c27c4a1c4803b679cc4e6305703
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/16/2020
ms.locfileid: "48489045"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="0de44-102">OneDrive Iş 'te depolamayı arttırma</span><span class="sxs-lookup"><span data-stu-id="0de44-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="0de44-103">Yeni ve var olan OneDrive kullanıcılarının varsayılan depolamasını değiştirmek için:</span><span class="sxs-lookup"><span data-stu-id="0de44-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="0de44-104">[OneDrive yönetim merkezinin depolama sayfasına](https://admin.onedrive.com/?v=StorageSettings)gıdın, GB cinsinden yeni bir miktar girin ve **Kaydet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="0de44-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), enter a new amount in GB, then select **Save**.</span></span>

<span data-ttu-id="0de44-105">Bu depolama alanı ayarı, belirli depolama sınırları ayarlamadığınız tüm kullanıcılara uygulanır.</span><span class="sxs-lookup"><span data-stu-id="0de44-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="0de44-106">Belirli kullanıcıların depolama alanını değiştirmek için Microsoft PowerShell 'i kullanın.</span><span class="sxs-lookup"><span data-stu-id="0de44-106">To change the storage space for specific users, use Microsoft PowerShell.</span></span> <span data-ttu-id="0de44-107">Bunun nasıl yapılacağı hakkında bilgi için, [PowerShell kullanarak kullanıcılarınızın OneDrive depolama alanını değiştirme](https://docs.microsoft.com/onedrive/change-user-storage)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="0de44-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://docs.microsoft.com/onedrive/change-user-storage).</span></span>

<span data-ttu-id="0de44-108">**Not**: sınırsız depolama alanı içeren bir planınız yok gibi görünüyor.</span><span class="sxs-lookup"><span data-stu-id="0de44-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="0de44-109">Her planla birlikte gelen depolama alanı hakkında bilgi için, [OneDrive iş hizmeti açıklaması](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="0de44-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span></span>
  
<span data-ttu-id="0de44-110">OneDrive Iş 'te depolama alanınızı yükseltmek için, **OneDrive Iş plan 2** veya **Office 365 E3**içeren bir abonelik seçin.</span><span class="sxs-lookup"><span data-stu-id="0de44-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 E3**.</span></span>
  
<span data-ttu-id="0de44-111">Planları değiştirmek için, Yönetim merkezinde **Billing** \> [ürünlerinize](https://go.microsoft.com/fwlink/p/?linkid=842054) faturalandırma sayfasına gidin, değiştirilecek aboneliği seçin ve ardından **Kuruluşunuz için önerilen yükseltmeleri görüntüle**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="0de44-111">To change plans, in the admin center, go to the **Billing** \> [Your products](https://go.microsoft.com/fwlink/p/?linkid=842054) page, select the subscription to change, then choose **View upgrades recommended for your org**.</span></span>
  
<span data-ttu-id="0de44-112">Plan değiştirme ve OneDrive Iş depolama hakkında daha fazla bilgi için bkz: [farklı bir plana](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan) ve [OneDrive Iş hizmeti açıklamasına](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description)yükseltme.</span><span class="sxs-lookup"><span data-stu-id="0de44-112">For more information on changing plans and OneDrive for Business storage, see [Upgrade to a different plan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan) and the [OneDrive for Business Service Description](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span></span>