---
title: İzinleri devralma
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 8/7/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: 5a72a74710a01cf958fa468b80ee67a4034c4383
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30752222"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="6de06-102">İzinlerin devralınmasını SharePoint'te nasıl çalışır?</span><span class="sxs-lookup"><span data-stu-id="6de06-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="6de06-103">Varsayılan olarak, SharePoint izinleri sıradüzeninde daha yüksek up dan devralınır.</span><span class="sxs-lookup"><span data-stu-id="6de06-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="6de06-104">Bu nedenle dosya izinlerini site koleksiyonundan devralınan site izinlerini devralır kitaplığı izinlerini devralır klasöründen kendi izinleri devralır.</span><span class="sxs-lookup"><span data-stu-id="6de06-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="6de06-105">[Düzenleyebilir ve bir liste veya kitaplık izinlerini yönetmek](https://go.microsoft.com/fwlink/?linkid=869946)kaldırma benzersiz izinler ve devralma geri yükleme hakkında daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="6de06-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

