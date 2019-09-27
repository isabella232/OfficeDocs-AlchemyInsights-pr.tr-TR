---
title: Veri konumu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207281"
---
# <a name="data-location"></a><span data-ttu-id="18f06-102">Veri konumu</span><span class="sxs-lookup"><span data-stu-id="18f06-102">Data location</span></span>

<span data-ttu-id="18f06-103">Yönetici merkezinde veya PowerShell üzerinden Exchange Online'a bağlanarak Office 365 kiracınızın konumunu görüntüleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="18f06-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="18f06-104">**Yönetici merkezi:**</span><span class="sxs-lookup"><span data-stu-id="18f06-104">**Admin center:**</span></span>
1. <span data-ttu-id="18f06-105">[Yönetici merkezine](https://admin.microsoft.com/Adminportal/Home)giriş yapın.</span><span class="sxs-lookup"><span data-stu-id="18f06-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="18f06-106">**Ayarlar** > **Organizasyonu profilini**seçin.</span><span class="sxs-lookup"><span data-stu-id="18f06-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="18f06-107">**Veri konumu**altında, **ayrıntıları görüntüle'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="18f06-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="18f06-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="18f06-108">**PowerShell:**</span></span>
1. <span data-ttu-id="18f06-109">Windows PowerShell'i kullanarak Exchange Online'a bağlanın.</span><span class="sxs-lookup"><span data-stu-id="18f06-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="18f06-110">Kiracınızın özelliklerinin listesini görüntülemek için [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet'i çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="18f06-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="18f06-111">OrganizationId özelliğine bakın.</span><span class="sxs-lookup"><span data-stu-id="18f06-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="18f06-112">EXO ve SPO için veri konumuna sahip olduğunuzda, [verilerinizin bulunduğu yerden](https://products.office.com/where-is-your-data-located)kullanabileceğiniz diğer hizmetlerin veri konumunu belirleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="18f06-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>