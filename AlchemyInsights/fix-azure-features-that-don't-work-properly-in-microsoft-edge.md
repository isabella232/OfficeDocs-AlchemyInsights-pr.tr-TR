---
title: Azure özellikleri Microsoft Edge 'de düzgün çalışmazsa ne yapmalısınız?
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583779"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="ccf4a-102">Azure özellikleri Microsoft Edge 'de düzgün çalışmazsa ne yapmalısınız?</span><span class="sxs-lookup"><span data-stu-id="ccf4a-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="ccf4a-103">Microsoft Edge, güvenlik bölgeleriyle ilgili [bilinen sorunlarla karşılaşmıştır](https://go.microsoft.com/fwlink/?linkid=2140608) ve Azure kullanıcılarının Windows Yönetim Merkezi 'nde oturum açmasını etkileyebilir.</span><span class="sxs-lookup"><span data-stu-id="ccf4a-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="ccf4a-104">Microsoft Edge ile Azure özelliklerini kullanırken sorun yaşıyorsanız aşağıdaki adımları deneyin:</span><span class="sxs-lookup"><span data-stu-id="ccf4a-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="ccf4a-105">**Başlat** menüsünde **Internet seçenekleri** 'ni arayın ve seçin.</span><span class="sxs-lookup"><span data-stu-id="ccf4a-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="ccf4a-106">**Internet özellikleri** iletişim kutusunda, **güvenlik** sekmesine gidin.</span><span class="sxs-lookup"><span data-stu-id="ccf4a-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="ccf4a-107">**Güvenilen siteler** bölgesini seçin ve sonra **siteler** düğmesini seçin.</span><span class="sxs-lookup"><span data-stu-id="ccf4a-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="ccf4a-108">**Güvenilen siteler** iletişim kutusunda, ağ geçidi URL 'sini olduğu gibi [https://login.microsoftonline.com](https://login.microsoftonline.com) ve [https://login.live.com](https://login.live.com) ardından da **Kapat**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="ccf4a-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="ccf4a-109">**Internet özellikleri** Iletişim kutusunda **Gizlilik** sekmesine gidin.</span><span class="sxs-lookup"><span data-stu-id="ccf4a-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="ccf4a-110">Açılır pencere **Engelleyicisi** bölümünde **Ayarlar**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="ccf4a-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="ccf4a-111">Açılan iletişim kutusunda, ve ile ağ geçidi URL 'sini [https://login.microsoftonline.com](https://login.microsoftonline.com) ve [https://login.live.com](https://login.live.com) ardından da **Kapat**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="ccf4a-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
