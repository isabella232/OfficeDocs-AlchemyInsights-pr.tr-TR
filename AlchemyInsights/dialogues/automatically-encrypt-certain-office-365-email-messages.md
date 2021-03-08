---
title: Bazı Office 365 e-posta iletilerini otomatik olarak şifrele
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527614"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="b578a-102">Bazı Office 365 e-posta iletilerini otomatik olarak şifrele</span><span class="sxs-lookup"><span data-stu-id="b578a-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="b578a-103">Kullanıcıların bazı dış kişi veya kuruluşlara göndertilen iletileri otomatik olarak şifrelersiniz.</span><span class="sxs-lookup"><span data-stu-id="b578a-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="b578a-104">Bunu yapmak için aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="b578a-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="b578a-105">Exchange yönetim [merkezinde posta](https://outlook.office365.com/ecp/)akışı yönetim **> seçin.**</span><span class="sxs-lookup"><span data-stu-id="b578a-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="b578a-106">Yeni **(+) simgesine** tıklayın ve sonra iletilere **Office 365 İleti Şifrelemesi ve hak koruması uygula'ya tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="b578a-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="b578a-107">Ad **alanına** kural için bir ad girin; örneğin, *E-postaya gönderilen iletileri DrToniRamos@gmail.com.*</span><span class="sxs-lookup"><span data-stu-id="b578a-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="b578a-108">Bu **kuralı uygula'da,** bu **kişinin alıcı > seçin.**</span><span class="sxs-lookup"><span data-stu-id="b578a-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="b578a-109">Üyeleri **Seç penceresinde,** şifreleme kuralının uygulamak istediğiniz kişinin adını seçin ve ekle'ye **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="b578a-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="b578a-110">Kullanıcı eklemeyi bitirerek Tamam'a **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="b578a-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="b578a-111">Aşağıdaki do **alanını yanında, Birini** **seç'i tıklatın.**</span><span class="sxs-lookup"><span data-stu-id="b578a-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="b578a-112">RMS şablonu **açılan menüsünde** Şifrele'yi seçin **ve** Tamam'a **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="b578a-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="b578a-113">(Bu seçeneği görmüyorsanız, planınız otomatik şifreleme içermesi anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="b578a-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="b578a-114">Ancak add it!)</span><span class="sxs-lookup"><span data-stu-id="b578a-114">But you can add it!)</span></span>
9. <span data-ttu-id="b578a-115">İsteğe bağlı herhangi bir seçim seçin (bu noktada, çoğu basitlik için varsayılan ayarla bırakıla birlikte bırakabilirsiniz) isteğe bağlı seçimler listesinden seçim yapın.</span><span class="sxs-lookup"><span data-stu-id="b578a-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="b578a-116">**Kaydet**’e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="b578a-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b578a-117">Daha sonra istediğiniz zaman geri gelebilir ve bu kuralı düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b578a-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="b578a-118">Şifreleme kuralları oluşturma hakkında daha fazla bilgi için bkz. [Office 365'te](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)e-posta iletilerini şifrelemek için posta akışı kurallarını tanımlama.</span><span class="sxs-lookup"><span data-stu-id="b578a-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

