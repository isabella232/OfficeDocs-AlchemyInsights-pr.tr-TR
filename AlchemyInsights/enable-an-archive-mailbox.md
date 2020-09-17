---
title: Arşiv posta kutusunu etkinleştirme
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811726"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="422f7-102">Arşiv posta kutusunu etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="422f7-102">Enable an archive mailbox</span></span>

<span data-ttu-id="422f7-103">Arşiv posta kutusunun yapılandırılmasını sağlamak için otomatik denetimler 'in çalıştırılmasını istiyorsanız, bu sayfanın en üstündeki geri düğmesini < seçin ve ardından hesabın e-posta adresini girin.</span><span class="sxs-lookup"><span data-stu-id="422f7-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="422f7-104">Microsoft 365 'da posta kutularını arşivleme ( *Çevrimiçi Arşivler* veya *yerinde Arşivler*olarak da bilinir) kullanıcılara ek e-posta deposu sağlar.</span><span class="sxs-lookup"><span data-stu-id="422f7-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="422f7-105">Kullanıcılar öğeleri arşiv posta kutularına taşıyabilir veya kopyalayabilir ve yöneticiler öğeleri otomatik olarak arşiv posta kutularına taşıyan bir arşiv ilkesi oluşturabilir.</span><span class="sxs-lookup"><span data-stu-id="422f7-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="422f7-106">Arşiv posta kutusu şöyle oluşturulur:</span><span class="sxs-lookup"><span data-stu-id="422f7-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="422f7-107">[https://protection.office.com](https://protection.office.com) adımına gidin.</span><span class="sxs-lookup"><span data-stu-id="422f7-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="422f7-108">Yönetici hesabınızı kullanarak Microsoft 365 oturumu açın.</span><span class="sxs-lookup"><span data-stu-id="422f7-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="422f7-109">Güvenlik Uyumluluk Merkezi 'nin sol bölmesinde &amp; **bilgi** Yönetim \> **Arşivi**'ni seçin.</span><span class="sxs-lookup"><span data-stu-id="422f7-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="422f7-110">Arşiv posta kutusunu etkinleştirmek istediğiniz kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="422f7-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="422f7-111">Sağdaki Ayrıntılar bölmesinde, **Etkinleştir** 'e tıklayın ve sonra da arşiv posta kutusunu etkinleştirmek için uyarı Iletisinde **Evet 'e** tıklayın.</span><span class="sxs-lookup"><span data-stu-id="422f7-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="422f7-112">Ayrıca, birden çok kullanıcı seçerek ( **SHIFT** veya **CTRL** tuşlarını kullanarak) ve ardından Ayrıntılar bölmesinde **Etkinleştir** 'e tıklayarak arşiv posta kutularını toplu olarak etkinleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="422f7-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="422f7-113">Paylaşılan posta kutuları</span><span class="sxs-lookup"><span data-stu-id="422f7-113">Shared mailboxes</span></span>

<span data-ttu-id="422f7-114">Paylaşılan bir posta kutusunun arşivini etkinleştirmek için, Exchange Online arşivleme lisansıyla bir Exchange Online Plan 2 lisansı veya Exchange Online Plan 1 lisansı gereklidir.</span><span class="sxs-lookup"><span data-stu-id="422f7-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="422f7-115">Paylaşılan posta kutusunun arşivini etkinleştirmek için:</span><span class="sxs-lookup"><span data-stu-id="422f7-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="422f7-116">[Exchange Yönetim merkezine](https://outlook.office365.com/ecp) gidin ve yönetici hesabınızı kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="422f7-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="422f7-117">Paylaşılan **Alıcılar**'a gidin  >  **Shared**.</span><span class="sxs-lookup"><span data-stu-id="422f7-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="422f7-118">Paylaşılan posta kutusunu seçin.</span><span class="sxs-lookup"><span data-stu-id="422f7-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="422f7-119">Sağdaki Ayrıntılar bölmesinde, **yerinde arşiv**altında, **Etkinleştir**'i ve ardından arşiv posta kutusunu etkinleştirmek için **Evet** 'i tıklatın.</span><span class="sxs-lookup"><span data-stu-id="422f7-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="422f7-120">Daha fazla bilgi için bkz.:</span><span class="sxs-lookup"><span data-stu-id="422f7-120">For more information, see:</span></span>
  
- [<span data-ttu-id="422f7-121">Arşiv posta kutularını etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="422f7-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="422f7-122">Arşiv ve silme ilkesi ayarlama</span><span class="sxs-lookup"><span data-stu-id="422f7-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
