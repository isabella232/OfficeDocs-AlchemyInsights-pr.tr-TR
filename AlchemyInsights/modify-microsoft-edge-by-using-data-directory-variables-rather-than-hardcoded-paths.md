---
title: Microsoft Edge 'i, kodlanmış yollar yerine veri dizini değişkenlerini kullanarak değiştirme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679155"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a><span data-ttu-id="a1890-102">Microsoft Edge 'i, kodlanmış yollar yerine veri dizini değişkenlerini kullanarak değiştirme</span><span class="sxs-lookup"><span data-stu-id="a1890-102">Modify Microsoft Edge by using data directory variables rather than hardcoded paths</span></span>

<span data-ttu-id="a1890-103">Örneğin, Windows 'da, profil verilerini varsayılan konum yerine kullanıcının yerel uygulama verilerinin altında depolamak için **Userdatadir** ilkesini **$ {local_app_data} \Edge\Profile** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="a1890-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the **UserDataDir** policy to **${local_app_data}\Edge\Profile**.</span></span> 

<span data-ttu-id="a1890-104">Daha fazla bilgi edinmek için [Microsoft Edge Kullanıcı veri dizini değişkenleri oluşturma](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="a1890-104">To learn more, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).</span></span>