---
title: Exchange Yönetim merkezinde bekletme Ilkeleri çalışmıyor
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740530"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="8eeab-102">Exchange Yönetim merkezinde bekletme Ilkeleri</span><span class="sxs-lookup"><span data-stu-id="8eeab-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="8eeab-103">Aşağıda belirtilen ayarlar için otomatik denetimler 'in çalıştırılmasını istiyorsanız, bu sayfanın en üstündeki geri düğmesini < seçin ve ardından bekletme ilkeleriyle ilgili sorun olan kullanıcının e-posta adresini girin.</span><span class="sxs-lookup"><span data-stu-id="8eeab-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="8eeab-104">**Sorun:** Exchange Yönetim merkezinde yeni oluşturulan veya güncelleştirilen bekletme ilkeleri posta kutularına veya öğeler arşiv posta kutusuna taşınmaz veya silinir.</span><span class="sxs-lookup"><span data-stu-id="8eeab-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="8eeab-105">**Kök nedenler:**</span><span class="sxs-lookup"><span data-stu-id="8eeab-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="8eeab-106">Bu, **yönetilen klasör Yardımcısı 'nın** kullanıcının posta kutusunu işlemediği için olabilir.</span><span class="sxs-lookup"><span data-stu-id="8eeab-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="8eeab-107">Yönetilen klasör Yardımcısı, bulut tabanlı kuruluşunuzdaki her posta kutusunu yedi günde bir kez işlemeye çalışır.</span><span class="sxs-lookup"><span data-stu-id="8eeab-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="8eeab-108">Bir bekletme etiketini değiştirir veya posta kutusuna farklı bir bekletme ilkesi uygularsanız, yönetilen klasör Yardımcısı 'Nın posta kutusunu işlemesini bekleyebilirsiniz veya belirli bir posta kutusunu işlemek üzere yönetilen klasör Yardımcısı 'nı başlatmak için Start-ManagedFolderAssistant cmdlet 'ini çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8eeab-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="8eeab-109">Bu cmdlet 'i çalıştırmak, bekletme ilkesi veya bekletme etiketi ayarlarını sınamak veya sorun gidermek için kullanışlıdır.</span><span class="sxs-lookup"><span data-stu-id="8eeab-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="8eeab-110">Daha fazla bilgi için [yönetilen klasör Yardımcısı 'Nı çalıştırmayı](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)ziyaret edin.</span><span class="sxs-lookup"><span data-stu-id="8eeab-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="8eeab-111">**Çözüm:** Belirli bir posta kutusunun yönetilen klasör Yardımcısı 'nı başlatmak için aşağıdaki komutu çalıştırarak:</span><span class="sxs-lookup"><span data-stu-id="8eeab-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="8eeab-112">**RetentionHold** , posta kutusunda **etkinleştirilmişse** da bu olabilir.</span><span class="sxs-lookup"><span data-stu-id="8eeab-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="8eeab-113">Posta kutusu bir RetentionHold üzerine yerleştirilmişse, bu süre içinde posta kutusundaki bekletme ilkesi işlenmeyecektir.</span><span class="sxs-lookup"><span data-stu-id="8eeab-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="8eeab-114">RetentionHold ayarında daha fazla bilgi için [bkz.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="8eeab-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="8eeab-115">**Çözümlerden**</span><span class="sxs-lookup"><span data-stu-id="8eeab-115">**Solution:**</span></span>
    
  - <span data-ttu-id="8eeab-116">[Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)'teki belirli bir posta kutusundaki RetentionHold ayarının durumunu denetleyin:</span><span class="sxs-lookup"><span data-stu-id="8eeab-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="8eeab-117">Belirli bir posta kutusunda RetentionHold **devre dışı bırakmak** için aşağıdaki komutu bırakın:</span><span class="sxs-lookup"><span data-stu-id="8eeab-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="8eeab-118">Şimdi, yönetilen klasör Yardımcısı 'nı yeniden çalıştırarak:</span><span class="sxs-lookup"><span data-stu-id="8eeab-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="8eeab-119">**Not:** Posta kutusu 10 MB 'den küçükse, yönetilen klasör Yardımcısı posta kutusunu otomatik olarak işlemez.</span><span class="sxs-lookup"><span data-stu-id="8eeab-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="8eeab-120">Exchange Yönetim merkezinde bekletme ilkeleri hakkında daha fazla bilgi için bkz:</span><span class="sxs-lookup"><span data-stu-id="8eeab-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="8eeab-121">Bekletme etiketleri ve bekletme ilkeleri</span><span class="sxs-lookup"><span data-stu-id="8eeab-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="8eeab-122">Posta kutularına bekletme ilkesi uygulama</span><span class="sxs-lookup"><span data-stu-id="8eeab-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="8eeab-123">Bekletme etiketlerini ekleme veya kaldırma</span><span class="sxs-lookup"><span data-stu-id="8eeab-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="8eeab-124">Posta kutusuna yerleştirilen bekletme türlerini tanımlama</span><span class="sxs-lookup"><span data-stu-id="8eeab-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
