---
title: Bekletme ilkeleri Exchange Yönetim Merkezi çalışmıyor
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 73e8db432afccb73b872ec7a3ce84c25f1ba7f25
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786790"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="9eb0d-102">Exchange Yönetim Merkezi'nde bekletme ilkeleri</span><span class="sxs-lookup"><span data-stu-id="9eb0d-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="9eb0d-103">**Sorun:** Yeni oluşturulan veya posta kutularına Exchange Yönetim Merkezi'ndeki güncelleştirilmiş bekletme ilkeleri yapmamayı veya öğeleri değil arşiv posta kutusuna taşınmış veya silinmiş.</span><span class="sxs-lookup"><span data-stu-id="9eb0d-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="9eb0d-104">**Ana nedenler:**</span><span class="sxs-lookup"><span data-stu-id="9eb0d-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="9eb0d-p101">**Klasör Yardımcısı yönetilen** kullanıcının posta işlenmemiş olan nedeni bu olabilir. Her posta kutusu bulut tabanlı, kuruluşunuzdaki her yedi günde işlemek Yönetilen Klasör Yardımcısı çalışır. Bekletme etiketi değiştirmek ya da bir posta kutusu için farklı bir bekletme ilkesi uygulayın, posta kutusunu işleyen Yönetilen Klasör Yardımcısı veya yönetilen klasör belirli bir işlem için Yardımcısı'nı başlatmak için Başlat-ManagedFolderAssistant cmdlet'i çalıştırabilirsiniz kadar bekleyebilirsiniz posta kutusu. Bu cmdlet'i çalıştırmak sınama veya bir bekletme ilkesi veya bekletme etiket ayarları sorun giderme için yararlı olacaktır. Daha fazla bilgi için ziyaret edin [Yönetilen Klasör Yardımcısı'nı çalıştırın](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="9eb0d-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="9eb0d-110">**Çözüm:** Yönetilen Klasör Yardımcısı belirli bir posta kutusu için başlatmak için aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="9eb0d-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="9eb0d-p102">Bu da olması oluşabilir **RetentionHold** posta kutusu **Etkin** hale getirildi. Posta kutusu bir RetentionHold konduysa, posta kutusunun üzerinde bekletme ilkesini bu süre içinde işlenmez. RetentionHold ayar bkz: hakkında daha fazla bilgilerini için: [Posta kutusu saklama tutun](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="9eb0d-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="9eb0d-114">**Çözüm:**</span><span class="sxs-lookup"><span data-stu-id="9eb0d-114">**Solution:**</span></span>
    
  - <span data-ttu-id="9eb0d-115">RetentionHold ayarı belirli bir posta kutusu [EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)PowerShell'de durumunu denetleyin:</span><span class="sxs-lookup"><span data-stu-id="9eb0d-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="9eb0d-116">Belirli bir posta kutusuna RetentionHold **devre dışı bırakmak** için aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="9eb0d-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="9eb0d-117">Şimdi, yönetilen Klasör Yardımcısı'nı yeniden çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="9eb0d-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="9eb0d-118">**Not:** Posta kutusu 10 MB'den küçükse, yönetilen Klasör Yardımcısı otomatik olarak posta kutusu işlemez.</span><span class="sxs-lookup"><span data-stu-id="9eb0d-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

