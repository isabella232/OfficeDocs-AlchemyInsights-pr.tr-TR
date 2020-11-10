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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982554"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="b7c8f-102">Liste öğeleri hakkında açıklamalar</span><span class="sxs-lookup"><span data-stu-id="b7c8f-102">Comments on List items</span></span>

<span data-ttu-id="b7c8f-103">Kullanıcılar yakında liste öğelerine açıklama ekleyebilir ve bunları silebilir.</span><span class="sxs-lookup"><span data-stu-id="b7c8f-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="b7c8f-104">Kullanıcılar liste öğesindeki tüm açıklamaları görüntüleyebilir ve öğeyle ilgili açıklamaları veya etkinlikleri gösteren görünümler arasında filtre uygulayabilir.</span><span class="sxs-lookup"><span data-stu-id="b7c8f-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="b7c8f-105">**Zamanlama** :</span><span class="sxs-lookup"><span data-stu-id="b7c8f-105">**Timing** :</span></span>

<span data-ttu-id="b7c8f-106">**Hedeflenen sürüm** : orta Ekim 'de dereceli olarak alınan ve PARÇAAL-Kasım tarafından tamamlanması beklenen</span><span class="sxs-lookup"><span data-stu-id="b7c8f-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="b7c8f-107">**Standart sürüm** : PARÇAAL-Kasım ' da aşamalı toplama ve ilk Aralık ile tamamlanması bekleniyor</span><span class="sxs-lookup"><span data-stu-id="b7c8f-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="b7c8f-108">Kuruluş **: kuruluşun** tamamı için hedeflenen sürüm</span><span class="sxs-lookup"><span data-stu-id="b7c8f-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="b7c8f-109">Kullanıcıların açıklamaları ekleyip silebilmeleri için aşağıdakileri not etmeleri gerekir:</span><span class="sxs-lookup"><span data-stu-id="b7c8f-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="b7c8f-110">Açıklamalar SharePoint 'te devralınan izin ayarlarını izler.</span><span class="sxs-lookup"><span data-stu-id="b7c8f-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="b7c8f-111">Görev listeleri gibi modern kullanıcı arabirimlerinde gösterilecek henüz oluşturulmamış klasik listeler bu yorum özelliğini içermez.</span><span class="sxs-lookup"><span data-stu-id="b7c8f-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="b7c8f-112">Ekipte bulunan listelere açıklama eklemek bu sürümde kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="b7c8f-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="b7c8f-113">Açıklamalar, arama tarafından dizine alınır.</span><span class="sxs-lookup"><span data-stu-id="b7c8f-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="b7c8f-114">Yöneticiler, **set-SPOTenant** PowerShell cmdlet 'inde **CommentsOnListItemsDisabled** parametresini değiştirerek bu özelliği kuruluş düzeyinde devre dışı bırakabilir.</span><span class="sxs-lookup"><span data-stu-id="b7c8f-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="b7c8f-115">Site veya liste düzeyinde açıklama oluşturmayı devre dışı bırakmak mümkün değildir.</span><span class="sxs-lookup"><span data-stu-id="b7c8f-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="b7c8f-116">Bu denetimlerin, büyük olasılıkla ilk çeyrek 2021 bu denetimlerden bir sonraki güncelleştirmede da yer almak isteriz.</span><span class="sxs-lookup"><span data-stu-id="b7c8f-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
