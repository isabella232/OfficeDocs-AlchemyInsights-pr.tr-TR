---
title: E-posta iletilerini arşiv posta kutusuna taşıma
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799800"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="06771-102">E-postayı arşiv posta kutusuna taşıma</span><span class="sxs-lookup"><span data-stu-id="06771-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="06771-103">Aşağıda belirtilen ayarlar için otomatik denetimler 'in çalıştırılmasını istiyorsanız, bu sayfanın en üstündeki geri düğmesini < seçin ve ardından e-postayı arşiv posta kutularına taşıma sorunlarını yaşayan kullanıcının e-posta adresini girin.</span><span class="sxs-lookup"><span data-stu-id="06771-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="06771-104">**Arşiv posta kutusunun** etkinleştirildiğini onaylayın.</span><span class="sxs-lookup"><span data-stu-id="06771-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="06771-105">Yoksa, [Bu makaledeki](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) adımları kullanarak arşiv posta kutusunu etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="06771-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="06771-106">İletileri otomatik olarak arşiv posta kutusuna arşivlemek için, **arşive taşı** eylemine sahip bir bekletme etiketi, **posta kutusu (varsayılan) etiketine otomatik olarak uygulanacak**şekilde ayarlanmalıdır.</span><span class="sxs-lookup"><span data-stu-id="06771-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="06771-107">Etiket: [Arşiv varsayılan etiketini](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)oluşturmak için buradaki adımları kullanın.</span><span class="sxs-lookup"><span data-stu-id="06771-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="06771-108">Ardından, **Arşiv** etiketini bekletme ilkeniz ekleyin.</span><span class="sxs-lookup"><span data-stu-id="06771-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="06771-109">Exchange Yönetim merkezinde **bekletme ilkeleri** 'ni seçin > Kaydet **'e taşı etiketini** **Kaydet > kaydedin**.</span><span class="sxs-lookup"><span data-stu-id="06771-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="06771-110">Artık [bekletme ilkesini](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) belirli bir kullanıcının posta kutusuna atayın.</span><span class="sxs-lookup"><span data-stu-id="06771-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="06771-111">Aynı ilke hem **birincil** hem de **Arşiv** posta kutusuna uygulanacaktır.</span><span class="sxs-lookup"><span data-stu-id="06771-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="06771-112">Yönetilen klasör Yardımcısı (MFA) çalıştırmak ve yeni ayarları kullanıcının posta kutusuna uygulamak gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="06771-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="06771-113">Belirli bir posta kutusunun yönetilen klasör Yardımcısı 'nı başlatmak için [EXO PowerShell 'e bağlıyken](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) aşağıdaki komutu çalıştırırsınız:</span><span class="sxs-lookup"><span data-stu-id="06771-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="06771-114">Başlangıç-ManagedFolderAssistant-kimlik <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="06771-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="06771-115">Arşiv [ilkesi ayarlama hakkında](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="06771-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  