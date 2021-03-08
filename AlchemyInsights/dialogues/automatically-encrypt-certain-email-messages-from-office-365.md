---
title: Office 365'te bazı e-posta iletilerini otomatik olarak şifreleme
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527622"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="26dfe-102">Office 365'te bazı e-posta iletilerini otomatik olarak şifreleme</span><span class="sxs-lookup"><span data-stu-id="26dfe-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="26dfe-103">Exchange yönetim [merkezinde posta](https://outlook.office365.com/ecp/)akışı yönetim **> seçin.**</span><span class="sxs-lookup"><span data-stu-id="26dfe-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="26dfe-104">Yeni **(+) simgesine** tıklayın ve sonra iletilere **Office 365 İleti Şifrelemesi ve hak koruması uygula'ya tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="26dfe-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="26dfe-105">Ad **alanına** kural için bir ad girin; örneğin, Tüm *iletileri şifrele*.</span><span class="sxs-lookup"><span data-stu-id="26dfe-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="26dfe-106">Bu **kuralı uygula'da ,** **[Tüm iletilere uygula] seçin.**</span><span class="sxs-lookup"><span data-stu-id="26dfe-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="26dfe-107">Aşağıdaki do **alanını yanında, Birini** **seç'i tıklatın.**</span><span class="sxs-lookup"><span data-stu-id="26dfe-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="26dfe-108">RMS şablonu **açılan menüsünde** Şifrele'yi seçin **ve** Tamam'a **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="26dfe-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="26dfe-109">(Bu seçeneği görmüyorsanız, planınız otomatik şifreleme içermesi anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="26dfe-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="26dfe-110">Ancak add it!)</span><span class="sxs-lookup"><span data-stu-id="26dfe-110">But you can add it!)</span></span>
7. <span data-ttu-id="26dfe-111">Bu kuralı **önem düzeyi ile denetle onay** kutusunu işaretleyin ve sonra istediğiniz düzeyi seçin.</span><span class="sxs-lookup"><span data-stu-id="26dfe-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="26dfe-112">Şirketinizin tüm e-postaları şifrelenmiş olarak gönderme sözleşmeli yükümlülükleri varsa, düzeyi Yüksek olarak ayarlamanızı **öneririz.**</span><span class="sxs-lookup"><span data-stu-id="26dfe-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="26dfe-113">Bu **kural için model seçin altında Zorla'ya** **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="26dfe-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="26dfe-114">İsteğe bağlı herhangi bir seçim seçin (bu noktada, çoğu basitlik için varsayılan ayarla bırakıla birlikte bırakabilirsiniz) isteğe bağlı seçimler listesinden seçim yapın.</span><span class="sxs-lookup"><span data-stu-id="26dfe-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="26dfe-115">**Kaydet**’e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="26dfe-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="26dfe-116">Daha sonra istediğiniz zaman geri gelebilir ve bu kuralı düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="26dfe-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="26dfe-117">Şifreleme kuralları oluşturma hakkında daha fazla bilgi için, [Office 365'te](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) e-posta iletilerini şifrelemek için posta akışı kurallarını tanımlama</span><span class="sxs-lookup"><span data-stu-id="26dfe-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

