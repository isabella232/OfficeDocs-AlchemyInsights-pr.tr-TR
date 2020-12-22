---
title: Liste öğeleri hakkında açıklamalar
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
- "9003821"
- "6841"
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724174"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="6f58d-102">Liste öğeleri hakkında açıklamalar</span><span class="sxs-lookup"><span data-stu-id="6f58d-102">Comments on List items</span></span>

<span data-ttu-id="6f58d-103">Kullanıcılar liste öğesindeki tüm açıklamaları görüntüleyebilir ve öğeyle ilgili açıklamaları veya etkinlikleri gösteren görünümler arasında filtre uygulayabilir.</span><span class="sxs-lookup"><span data-stu-id="6f58d-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="6f58d-104">Kullanıcıların açıklamaları ekleyip silebilmeleri için aşağıdakileri not etmeleri gerekir:</span><span class="sxs-lookup"><span data-stu-id="6f58d-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="6f58d-105">Açıklamalar SharePoint 'te devralınan izin ayarlarını izler.</span><span class="sxs-lookup"><span data-stu-id="6f58d-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="6f58d-106">Görev listeleri gibi modern kullanıcı arabirimlerinde gösterilecek henüz oluşturulmamış klasik listeler bu yorum özelliğini içermez.</span><span class="sxs-lookup"><span data-stu-id="6f58d-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="6f58d-107">Ekipte bulunan listelere açıklama eklemek bu sürümde kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="6f58d-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="6f58d-108">Açıklamalar, arama tarafından dizine alınır.</span><span class="sxs-lookup"><span data-stu-id="6f58d-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="6f58d-109">Yöneticiler, **set-SPOTenant** PowerShell cmdlet 'inde **CommentsOnListItemsDisabled** parametresini değiştirerek bu özelliği kuruluş düzeyinde devre dışı bırakabilir.</span><span class="sxs-lookup"><span data-stu-id="6f58d-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="6f58d-110">Site veya liste düzeyinde açıklama oluşturmayı devre dışı bırakmak mümkün değildir.</span><span class="sxs-lookup"><span data-stu-id="6f58d-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="6f58d-111">Bu denetimlerin, büyük olasılıkla ilk çeyrek 2021 bu denetimlerden bir sonraki güncelleştirmede da yer almak isteriz.</span><span class="sxs-lookup"><span data-stu-id="6f58d-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
