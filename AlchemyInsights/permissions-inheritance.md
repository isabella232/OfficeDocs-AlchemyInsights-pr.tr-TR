---
title: İzinler devralma
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
ms.openlocfilehash: 6322ca12902be2612f65b6388a650300b257a95e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554984"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="df38d-102">SharePoint'te izinler devralma nasıl çalışır?</span><span class="sxs-lookup"><span data-stu-id="df38d-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="df38d-103">Varsayılan olarak, SharePoint'teki izinler hiyerarşide yukarıdan devralınır.</span><span class="sxs-lookup"><span data-stu-id="df38d-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="df38d-104">Bu nedenle bir dosya izinlerini, izinlerini site koleksiyonundan devralan siteden alan kitaplıktan devralan klasörden devralır.</span><span class="sxs-lookup"><span data-stu-id="df38d-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="df38d-105">Benzersiz izinleri kaldırma ve devralmayı geri alma hakkında bilgi için, [bir liste veya kitaplık için izinleri edin ve yönetin'](https://go.microsoft.com/fwlink/?linkid=869946)e bakın.</span><span class="sxs-lookup"><span data-stu-id="df38d-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

