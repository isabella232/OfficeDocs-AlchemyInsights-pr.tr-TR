---
title: E-posta iletilerini otomatik olarak arşiv posta kutusuna taşıma
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749292"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="55c63-102">E-posta iletilerini otomatik olarak arşiv posta kutusuna taşıma</span><span class="sxs-lookup"><span data-stu-id="55c63-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="55c63-103">Kullanıcının eski e-postalarını otomatik olarak arşiv posta kutusuna taşımak için ilke şöyle ayarlanır:</span><span class="sxs-lookup"><span data-stu-id="55c63-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="55c63-104">Kullanıcı için [**bir & posta kutusunun**](https://go.microsoft.com/fwlink/p/?linkid=2077143)etkinleştirildiğinden emin olmak için Güvenlik ve Uyumluluk  >    >   Verileri yönetimi Arşivi'ne gidin.</span><span class="sxs-lookup"><span data-stu-id="55c63-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="55c63-105">Açmamışsa, uyarı **kutusunda** Etkinleştir'e **ve** ardından Evet'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="55c63-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="55c63-106">Uyumluluk yönetimi [**ve bekletme etiketleri > Exchange > gidin.**](https://go.microsoft.com/fwlink/?linkid=2059104)</span><span class="sxs-lookup"><span data-stu-id="55c63-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="55c63-107">+ simgesini seçin ve ardından otomatik **olarak tüm posta kutusuna uygula'ya tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="55c63-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="55c63-108">Bekletme etiketine bir ad atayın ve Arşive **Taşı'ya seçin.**</span><span class="sxs-lookup"><span data-stu-id="55c63-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="55c63-109">Bekletme süresi için, 90 gün gibi istediğiniz saati girin.</span><span class="sxs-lookup"><span data-stu-id="55c63-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="55c63-110">**Kaydet**’e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="55c63-110">Click **Save**.</span></span>
5. <span data-ttu-id="55c63-111">Şimdi bir bekletme ilkesi oluşturun: bekletme **ilkelerini seçin,** yeni ilke eklemek için simgeyi seçin.</span><span class="sxs-lookup"><span data-stu-id="55c63-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="55c63-112">Bekletme ilkesine bir ad atamadıktan sonra, tıklar ve kaydırarak yeni oluşturduğunuz bekletme etiketini bulup ekleyin.</span><span class="sxs-lookup"><span data-stu-id="55c63-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="55c63-113">**Kaydet**’e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="55c63-113">Click **Save**.</span></span>
7. <span data-ttu-id="55c63-114">Son olarak, bekletme ilkesi kullanıcı posta kutusuna uygulanır: yine Exchange yönetim merkezinde, alıcıların posta  >  **kutularına gidin.**</span><span class="sxs-lookup"><span data-stu-id="55c63-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="55c63-115">İlkeyi uygulamak istediğiniz tüm kullanıcıları seçin, ardından Düzenle'yi **(kalem** simgesi) seçin.</span><span class="sxs-lookup"><span data-stu-id="55c63-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="55c63-116">İletişim kutusunda posta kutusu **özelliklerine tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="55c63-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="55c63-117">Bekletme **ilkesi'nin** altında, Yeni oluşturduğunuz ilkeyi > **kaydedin.**</span><span class="sxs-lookup"><span data-stu-id="55c63-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="55c63-118">İlkeyi tüm kullanıcılara uygulama yönergeleri için bkz. [Posta kutularına bekletme ilkesi uygulama.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)</span><span class="sxs-lookup"><span data-stu-id="55c63-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
