---
title: Belirli etki alanlarına gönderilen Office 365 e-posta iletilerini otomatik olarak şifreleme
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749297"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="81035-102">Belirli etki alanlarına gönderilen Office 365 e-posta iletilerini otomatik olarak şifreleme</span><span class="sxs-lookup"><span data-stu-id="81035-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="81035-103">Exchange yönetim [merkezinde posta](https://outlook.office365.com/ecp/)akışı yönetim **> seçin.**</span><span class="sxs-lookup"><span data-stu-id="81035-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="81035-104">Yeni **(+) simgesine** tıklayın ve sonra iletilere **Office 365 İleti Şifrelemesi ve hak koruması uygula'ya tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="81035-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="81035-105">Ad **alanına** kural için bir ad girin; örneğin, E-postaya gönderilen *iletileri contoso.com.*</span><span class="sxs-lookup"><span data-stu-id="81035-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="81035-106">Bu **kuralı uygula alanında, etki** alanının alıcı > **seçin.**</span><span class="sxs-lookup"><span data-stu-id="81035-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="81035-107">Etki alanının adını girin, **örneğin** contoso.com.</span><span class="sxs-lookup"><span data-stu-id="81035-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="81035-108">Ekle **(+) simgesine** ve ardından Tamam'a **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="81035-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="81035-109">Aşağıdaki do **alanını yanında, Birini** **seç'i tıklatın.**</span><span class="sxs-lookup"><span data-stu-id="81035-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="81035-110">RMS şablonu **açılan menüsünde** Şifrele'yi seçin **ve** Tamam'a **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="81035-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="81035-111">(Bu seçeneği görmüyorsanız, planınız otomatik şifreleme içermesi anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="81035-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="81035-112">Ancak add it!)</span><span class="sxs-lookup"><span data-stu-id="81035-112">But you can add it!)</span></span>
9. <span data-ttu-id="81035-113">İsteğe bağlı herhangi bir seçim seçin (bu noktada, çoğu basitlik için varsayılan ayarla bırakıla birlikte bırakabilirsiniz) isteğe bağlı seçimler listesinden seçim yapın.</span><span class="sxs-lookup"><span data-stu-id="81035-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="81035-114">**Kaydet**’e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="81035-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="81035-115">Daha sonra istediğiniz zaman geri gelebilir ve bu kuralı düzenleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="81035-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="81035-116">Şifreleme kuralları oluşturma hakkında daha fazla bilgi için, [Office 365'te](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) e-posta iletilerini şifrelemek için posta akışı kurallarını tanımlama</span><span class="sxs-lookup"><span data-stu-id="81035-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>