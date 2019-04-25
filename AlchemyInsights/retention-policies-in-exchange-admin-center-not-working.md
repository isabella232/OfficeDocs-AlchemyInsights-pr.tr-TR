---
title: Bekletme ilkeleri Exchange Yönetim Merkezi çalışmıyor
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371318"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="884b8-102">Exchange Yönetim Merkezi'nde bekletme ilkeleri</span><span class="sxs-lookup"><span data-stu-id="884b8-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="884b8-103">**Sorun:** Yeni oluşturulan veya posta kutularına Exchange Yönetim Merkezi'ndeki güncelleştirilmiş bekletme ilkeleri yapmamayı veya öğeleri değil arşiv posta kutusuna taşınmış veya silinmiş.</span><span class="sxs-lookup"><span data-stu-id="884b8-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="884b8-104">**Ana nedenler:**</span><span class="sxs-lookup"><span data-stu-id="884b8-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="884b8-105">**Klasör Yardımcısı yönetilen** kullanıcının posta işlenmemiş olan nedeni bu olabilir.</span><span class="sxs-lookup"><span data-stu-id="884b8-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="884b8-106">Her posta kutusu bulut tabanlı, kuruluşunuzdaki her yedi günde işlemek Yönetilen Klasör Yardımcısı çalışır.</span><span class="sxs-lookup"><span data-stu-id="884b8-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="884b8-107">Bekletme etiketi değiştirmek ya da bir posta kutusu için farklı bir bekletme ilkesi uygulayın, posta kutusunu işleyen Yönetilen Klasör Yardımcısı veya yönetilen klasör belirli bir işlem için Yardımcısı'nı başlatmak için Başlat-ManagedFolderAssistant cmdlet'i çalıştırabilirsiniz kadar bekleyebilirsiniz posta kutusu.</span><span class="sxs-lookup"><span data-stu-id="884b8-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="884b8-108">Bu cmdlet'i çalıştırmak sınama veya bir bekletme ilkesi veya bekletme etiket ayarları sorun giderme için yararlı olacaktır.</span><span class="sxs-lookup"><span data-stu-id="884b8-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="884b8-109">Daha fazla bilgi için ziyaret edin [Yönetilen Klasör Yardımcısı'nı çalıştırın](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="884b8-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="884b8-110">**Çözüm:** Yönetilen Klasör Yardımcısı belirli bir posta kutusu için başlatmak için aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="884b8-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="884b8-111">Bu da olması oluşabilir **RetentionHold** posta kutusu **Etkin** hale getirildi.</span><span class="sxs-lookup"><span data-stu-id="884b8-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="884b8-112">Posta kutusu bir RetentionHold konduysa, posta kutusunun üzerinde bekletme ilkesini bu süre içinde işlenmez.</span><span class="sxs-lookup"><span data-stu-id="884b8-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="884b8-113">RetentionHold ayar bkz: hakkında daha fazla bilgilerini için: [Posta kutusu saklama tutun](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="884b8-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="884b8-114">**Çözüm:**</span><span class="sxs-lookup"><span data-stu-id="884b8-114">**Solution:**</span></span>
    
  - <span data-ttu-id="884b8-115">RetentionHold ayarı belirli bir posta kutusu [EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)PowerShell'de durumunu denetleyin:</span><span class="sxs-lookup"><span data-stu-id="884b8-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="884b8-116">Belirli bir posta kutusuna RetentionHold **devre dışı bırakmak** için aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="884b8-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="884b8-117">Şimdi, yönetilen Klasör Yardımcısı'nı yeniden çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="884b8-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="884b8-118">**Not:** Posta kutusu 10 MB'den küçükse, yönetilen Klasör Yardımcısı otomatik olarak posta kutusu işlemez.</span><span class="sxs-lookup"><span data-stu-id="884b8-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

