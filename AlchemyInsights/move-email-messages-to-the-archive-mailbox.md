---
title: E-posta iletilerini Arşiv posta kutusuna taşıma
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511060"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="aafbe-102">E-postayı arşiv posta kutusuna taşıma</span><span class="sxs-lookup"><span data-stu-id="aafbe-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="aafbe-103">**Arşiv posta kutusunun** etkinleştirildiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="aafbe-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="aafbe-104">Değilse, arşiv posta kutusunu etkinleştirmek için [bu makaledeki](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) adımları kullanın.</span><span class="sxs-lookup"><span data-stu-id="aafbe-104">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="aafbe-105">İletileri arşiv posta kutusuna otomatik olarak arşivlemek için, **arşive taşı** eylemini içeren bir bekletme **etiketinin tüm posta kutusu (varsayılan) etiketine otomatik olarak uygulanacak**şekilde ayarlanması gerekir.</span><span class="sxs-lookup"><span data-stu-id="aafbe-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="aafbe-106">Etiketi oluşturmak için buradaki adımları kullanın: [Varsayılan etiketi ni arşivleyin.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)</span><span class="sxs-lookup"><span data-stu-id="aafbe-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="aafbe-107">Ardından, bekletme ilkenize **Arşiv** etiketini ekleyin.</span><span class="sxs-lookup"><span data-stu-id="aafbe-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="aafbe-108">Exchange yönetici merkezinde, **Bekletme İlkeleri'ni** seçin > **Kaydet**> ilkesine **Arşive Taşı etiketini** ekleyin.</span><span class="sxs-lookup"><span data-stu-id="aafbe-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="aafbe-109">Şimdi [Bekletme İlkesi'ni](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) belirli kullanıcının posta kutusuna atayın.</span><span class="sxs-lookup"><span data-stu-id="aafbe-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="aafbe-110">Aynı ilke hem **Birincil** hem de **Arşiv** posta kutusuna uygulanır.</span><span class="sxs-lookup"><span data-stu-id="aafbe-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="aafbe-111">Yönetilen Klasör Yardımcısı'nı (MFA) yeni ayarları çalıştırmaya ve kullanıcının posta kutusuna uygulamaya zorlamak gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="aafbe-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="aafbe-112">Belirli bir posta kutusu için Yönetilen Klasör Yardımcısı'nı başlatmak için [EXO PowerShell'e bağlıyken](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="aafbe-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="aafbe-113">Başlat-YönetilenFolderAssistant -Kimlik<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="aafbe-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="aafbe-114">Arşiv ilkesi ayarlama hakkında daha fazla bilgi için [bkz.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)</span><span class="sxs-lookup"><span data-stu-id="aafbe-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  