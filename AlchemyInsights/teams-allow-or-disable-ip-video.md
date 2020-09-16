---
title: Ekipler IP videosunu tanır veya devre dışı bırakır
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670204"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="6c2e9-102">Ekipler IP videosunu tanır veya devre dışı bırakır</span><span class="sxs-lookup"><span data-stu-id="6c2e9-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="6c2e9-103">**Toplantı ilkesini değiştirme veya oluşturma**</span><span class="sxs-lookup"><span data-stu-id="6c2e9-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="6c2e9-104">Toplantı ilkesini değiştirmek veya oluşturmak için, **Microsoft ekipleri yönetim merkezi > toplantılar > toplantı ilkelerine**gidin.</span><span class="sxs-lookup"><span data-stu-id="6c2e9-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="6c2e9-105">Listeden bir ilke seçin veya **Ekle**’ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6c2e9-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="6c2e9-106">Yeni ilke oluşturuyorsanız bir ad ve açıklama ekleyin.</span><span class="sxs-lookup"><span data-stu-id="6c2e9-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="6c2e9-107">Ad özel karakterler içeremez ve 64 karakterden uzun olamaz.</span><span class="sxs-lookup"><span data-stu-id="6c2e9-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="6c2e9-108">Ayarlarınızı seçin ve **Kaydet**'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6c2e9-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="6c2e9-109">Örneğin, birçok kullanıcınız olduğunu ve toplantılarının gerektirdiği bant genişliği miktarını sınırlandırmak istediğinizi varsayalım.</span><span class="sxs-lookup"><span data-stu-id="6c2e9-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="6c2e9-110">"Sınırlı bant genişliği" adlı yeni bir özel ilke oluşturabilir ve şu ayarları devre dışı bırakabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="6c2e9-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="6c2e9-111">**Ses ve görüntü**’nün altında:</span><span class="sxs-lookup"><span data-stu-id="6c2e9-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="6c2e9-112">Buluta kayda izin ver seçeneğini kapatın.</span><span class="sxs-lookup"><span data-stu-id="6c2e9-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="6c2e9-113">IP üzerinden videoya izin ver seçeneğini kapatın.</span><span class="sxs-lookup"><span data-stu-id="6c2e9-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="6c2e9-114">Sonra ilkeyi kullanıcılara atayın.</span><span class="sxs-lookup"><span data-stu-id="6c2e9-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="6c2e9-115">**Kullanıcılara toplantı ilkesi atama**</span><span class="sxs-lookup"><span data-stu-id="6c2e9-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="6c2e9-116">Microsoft Teams yönetim merkezinin sol gezintisinde **Kullanıcılar**’a gidin ve kullanıcıya tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6c2e9-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="6c2e9-117">Kullanıcı adının sol tarafına tıklayarak kullanıcıyı seçin ve ardından **Ayarları düzenle**’ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="6c2e9-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="6c2e9-118">**Toplantı ilkesi**altında, atamak istediğiniz ilkeyi seçin ve **Uygula**'yı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="6c2e9-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="6c2e9-119">Daha fazla bilgi için bkz [.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="6c2e9-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
