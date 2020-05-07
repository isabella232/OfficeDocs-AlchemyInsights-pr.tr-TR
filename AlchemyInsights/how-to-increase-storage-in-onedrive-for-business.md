---
title: OneDrive for Business'ta depolama alanı nasıl artırılabilen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: adee1c5d1ffc23f54580549ab666ee8fac579263
ms.sourcegitcommit: d1aad215f8aa636ba89c93a13a0c9d90e997f752
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/06/2020
ms.locfileid: "44063061"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="1ca29-102">OneDrive for Business'ta depolama alanı nasıl artırılabilen</span><span class="sxs-lookup"><span data-stu-id="1ca29-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="1ca29-103">Yeni ve mevcut OneDrive kullanıcıları için varsayılan depolama alanını değiştirmek için:</span><span class="sxs-lookup"><span data-stu-id="1ca29-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="1ca29-104">[OneDrive yönetici merkezinin Depolama sayfasına](https://admin.onedrive.com/?v=StorageSettings)gidin ve ardından GB olarak yeni bir tutar girin.</span><span class="sxs-lookup"><span data-stu-id="1ca29-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), and then enter a new amount in GB.</span></span>

<span data-ttu-id="1ca29-105">Bu depolama alanı ayarı, belirli depolama alanı sınırları belirlemediğiniz tüm kullanıcılar için geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="1ca29-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="1ca29-106">Belirli kullanıcıların depolama alanını değiştirmek için Microsoft PowerShell'i kullanmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="1ca29-106">To change the storage space for specific users, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="1ca29-107">Bunu nasıl yapacağınız hakkında bilgi için [PowerShell'i kullanarak kullanıcılarınızın OneDrive depolama alanını değiştir'e](https://go.microsoft.com/fwlink/?linkid=866402)bakın.</span><span class="sxs-lookup"><span data-stu-id="1ca29-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://go.microsoft.com/fwlink/?linkid=866402).</span></span>

<span data-ttu-id="1ca29-108">**NOT**: Sınırsız depolama içeren bir planınız yok gibi görünüyor.</span><span class="sxs-lookup"><span data-stu-id="1ca29-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="1ca29-109">Her planla birlikte gelen depolama alanı hakkında daha fazla bilgi için, [İş için OneDrive hizmet açıklamasına](https://go.microsoft.com/fwlink/p/?LinkID=826071)bakın.</span><span class="sxs-lookup"><span data-stu-id="1ca29-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://go.microsoft.com/fwlink/p/?LinkID=826071).</span></span>
  
<span data-ttu-id="1ca29-110">OneDrive for Business'taki depolama alanınızı artırmak için, **OneDrive for Business Plan 2** veya Office **365 Enterprise E3**içeren bir abonelik seçin.</span><span class="sxs-lookup"><span data-stu-id="1ca29-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 Enterprise E3**.</span></span> 
  
<span data-ttu-id="1ca29-111">Microsoft 365 yönetici merkezinde planları değiştirmek için, **[Ürünlerinizi](https://go.microsoft.com/fwlink/p/?linkid=842054)** **Faturalama** \> sayfasına gidin, değiştirmek için aboneliği seçin ve ardından **Yükseltme** sekmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="1ca29-111">To change plans, in the Microsoft 365 admin center, go to the **Billing** \> **[Your products](https://go.microsoft.com/fwlink/p/?linkid=842054)** page, select the subscription to change, and then choose the **Upgrade** tab.</span></span>
  
<span data-ttu-id="1ca29-112">Planlar ve OneDrive for Business depolama arasında geçiş hakkında daha fazla bilgi için, [iş planı için farklı bir Microsoft 365'e](https://go.microsoft.com/fwlink/?LinkId=2031117) ve İş Hizmeti Açıklaması için [OneDrive'a](https://go.microsoft.com/fwlink/p/?LinkId-2031122)geçiş bakın.</span><span class="sxs-lookup"><span data-stu-id="1ca29-112">For more information on switching plans and OneDrive for Business storage, see [Switch to a different Microsoft 365 for business plan](https://go.microsoft.com/fwlink/?LinkId=2031117) and the [OneDrive for Business Service Description](https://go.microsoft.com/fwlink/p/?LinkId-2031122).</span></span>