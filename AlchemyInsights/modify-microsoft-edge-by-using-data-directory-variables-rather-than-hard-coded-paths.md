---
title: Sabit kodlu yollar yerine veri dizini değişkenlerini kullanarak Microsoft Edge'i değiştirme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036860"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a><span data-ttu-id="023b6-102">Sabit kodlu yollar yerine veri dizini değişkenlerini kullanarak Microsoft Edge'i değiştirme</span><span class="sxs-lookup"><span data-stu-id="023b6-102">Modify Microsoft Edge by using data directory variables rather than hard-coded paths</span></span>

<span data-ttu-id="023b6-103">Örneğin, Windows'da profil verilerini varsayılan konum yerine kullanıcının yerel uygulama verileri altında depolamak *için, UserDataDir* ilkesini **${local_app_data}\Edge\Profile** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="023b6-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the *UserDataDir* policy to **${local_app_data}\Edge\Profile**.</span></span>

<span data-ttu-id="023b6-104">Daha fazla bilgi için [bkz. Microsoft Edge kullanıcı veri dizini değişkenleri oluşturma.](https://docs.microsoft.com/deployedge/microsoft-edge-policies)</span><span class="sxs-lookup"><span data-stu-id="023b6-104">For more information, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/microsoft-edge-policies).</span></span>