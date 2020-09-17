---
title: OneDrive Iş 'te depolamayı arttırma
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 53eabf6c87dead3b7309c7da1f8a590940127169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780115"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="1f603-102">OneDrive Iş 'te depolamayı arttırma</span><span class="sxs-lookup"><span data-stu-id="1f603-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="1f603-103">Yeni ve var olan OneDrive kullanıcılarının varsayılan depolamasını değiştirmek için:</span><span class="sxs-lookup"><span data-stu-id="1f603-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="1f603-104">[OneDrive yönetim merkezinin depolama sayfasına](https://admin.onedrive.com/?v=StorageSettings)gıdın ve GB cinsinden yeni miktarı girin.</span><span class="sxs-lookup"><span data-stu-id="1f603-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), and then enter a new amount in GB.</span></span>

<span data-ttu-id="1f603-105">Bu depolama alanı ayarı, belirli depolama sınırları ayarlamadığınız tüm kullanıcılara uygulanır.</span><span class="sxs-lookup"><span data-stu-id="1f603-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="1f603-106">Belirli kullanıcıların depolama alanını değiştirmek için Microsoft PowerShell kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="1f603-106">To change the storage space for specific users, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="1f603-107">Bunun nasıl yapılacağı hakkında bilgi için, [PowerShell kullanarak kullanıcılarınızın OneDrive depolama alanını değiştirme](https://go.microsoft.com/fwlink/?linkid=866402)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="1f603-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://go.microsoft.com/fwlink/?linkid=866402).</span></span>

<span data-ttu-id="1f603-108">**Not**: sınırsız depolama alanı içeren bir planınız yok gibi görünüyor.</span><span class="sxs-lookup"><span data-stu-id="1f603-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="1f603-109">Her planla birlikte gelen depolama alanı hakkında bilgi için, [OneDrive iş hizmeti açıklaması](https://go.microsoft.com/fwlink/p/?LinkID=826071)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="1f603-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://go.microsoft.com/fwlink/p/?LinkID=826071).</span></span>
  
<span data-ttu-id="1f603-110">OneDrive Iş 'te depolama alanınızı yükseltmek için, **OneDrive Iş plan 2** veya **Office 365 Kurumsal E3**'i içeren bir abonelik seçin.</span><span class="sxs-lookup"><span data-stu-id="1f603-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 Enterprise E3**.</span></span> 
  
<span data-ttu-id="1f603-111">Planları değiştirmek için, Microsoft 365 Yönetim merkezinde, **Billing** \> **[ürün](https://go.microsoft.com/fwlink/p/?linkid=842054)** faturalaması sayfasına gidin, değiştirilecek aboneliği seçin ve sonra da **Yükselt** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="1f603-111">To change plans, in the Microsoft 365 admin center, go to the **Billing** \> **[Your products](https://go.microsoft.com/fwlink/p/?linkid=842054)** page, select the subscription to change, and then choose the **Upgrade** tab.</span></span>
  
<span data-ttu-id="1f603-112">Plan değiştirme ve OneDrive Iş depolama hakkında daha fazla bilgi için bkz: [farklı bir Microsoft 365 iş planına geçme](https://go.microsoft.com/fwlink/?LinkId=2031117) ve [OneDrive iş servis açıklaması](https://go.microsoft.com/fwlink/p/?LinkId-2031122).</span><span class="sxs-lookup"><span data-stu-id="1f603-112">For more information on switching plans and OneDrive for Business storage, see [Switch to a different Microsoft 365 for business plan](https://go.microsoft.com/fwlink/?LinkId=2031117) and the [OneDrive for Business Service Description](https://go.microsoft.com/fwlink/p/?LinkId-2031122).</span></span>