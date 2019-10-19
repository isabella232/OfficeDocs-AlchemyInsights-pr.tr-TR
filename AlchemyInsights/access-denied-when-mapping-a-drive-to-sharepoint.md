---
title: Bir sürücüyü SharePoint'e eşleme yaparken erişim reddedildi
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: c41bfd9d25c8aa946a4ec5156be6d2424f4e2133
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737497"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="e01ac-102">Ağ sürücülerine eşlenen SharePoint kitaplıklarıyla ilgili sorunları düzeltme</span><span class="sxs-lookup"><span data-stu-id="e01ac-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="e01ac-103">Eşlenen bir ağ sürücüsüne göz attığınızda, aşağıdaki iletilerden birini görebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="e01ac-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="e01ac-104">**\\Yola erişilemez. Bu ağ kaynağını kullanma izniniz olmayabilir. Erişim izinlerinizin olup olmadığını öğrenmek için bu sunucunun yöneticisine başvurun.**</span><span class="sxs-lookup"><span data-stu-id="e01ac-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="e01ac-105">**Erişim Reddedildi. Bu konumda dosyaları açmadan önce, web sitesini önce güvenilen site listenize eklemeniz, web sitesine göz atmanız ve otomatik olarak oturum açma seçeneğini seçmeniz gerekir.**</span><span class="sxs-lookup"><span data-stu-id="e01ac-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="e01ac-106">[Eşlenen ağ sürücülerini sorun giderme yardımı alın.](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)</span><span class="sxs-lookup"><span data-stu-id="e01ac-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="e01ac-107">Kitaplığı ağ sürücüsü olarak eşleme geçicidir ve yalnızca Internet Explorer'da desteklenir.</span><span class="sxs-lookup"><span data-stu-id="e01ac-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="e01ac-108">Bunun yerine, SharePoint dosyalarını [İsteğe Bağlı Dosyalar](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)içeren [yeni OneDrive eşitleme istemcisiyle eşitleyin.](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx)</span><span class="sxs-lookup"><span data-stu-id="e01ac-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="e01ac-109">Yerel depolama alanı kullanmadan OneDrive'daki tüm dosyalarınıza erişin.</span><span class="sxs-lookup"><span data-stu-id="e01ac-109">Access all your files in OneDrive without using local storage space.</span></span>
  