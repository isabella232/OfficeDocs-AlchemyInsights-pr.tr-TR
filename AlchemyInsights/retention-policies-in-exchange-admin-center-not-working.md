---
title: Bekletme ilkeleri Exchange Yönetim Merkezi çalışmıyor
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551363"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange Yönetim Merkezi'nde bekletme ilkeleri

 **Sorun:** Yeni oluşturulan veya posta kutularına Exchange Yönetim Merkezi'ndeki güncelleştirilmiş bekletme ilkeleri yapmamayı veya öğeleri değil arşiv posta kutusuna taşınmış veya silinmiş. 
  
 **Ana nedenler:**
  
- **Klasör Yardımcısı yönetilen** kullanıcının posta işlenmemiş olan nedeni bu olabilir. Her posta kutusu bulut tabanlı, kuruluşunuzdaki her yedi günde işlemek Yönetilen Klasör Yardımcısı çalışır. Bekletme etiketi değiştirmek ya da bir posta kutusu için farklı bir bekletme ilkesi uygulayın, posta kutusunu işleyen Yönetilen Klasör Yardımcısı veya yönetilen klasör belirli bir işlem için Yardımcısı'nı başlatmak için Başlat-ManagedFolderAssistant cmdlet'i çalıştırabilirsiniz kadar bekleyebilirsiniz posta kutusu. Bu cmdlet'i çalıştırmak sınama veya bir bekletme ilkesi veya bekletme etiket ayarları sorun giderme için yararlı olacaktır. Daha fazla bilgi için ziyaret edin [Yönetilen Klasör Yardımcısı'nı çalıştırın](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Çözüm:** Yönetilen Klasör Yardımcısı belirli bir posta kutusu için başlatmak için aşağıdaki komutu çalıştırın:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Bu da olması oluşabilir **RetentionHold** posta kutusu **Etkin** hale getirildi. Posta kutusu bir RetentionHold konduysa, posta kutusunun üzerinde bekletme ilkesini bu süre içinde işlenmez. RetentionHold ayar bkz: hakkında daha fazla bilgilerini için: [Posta kutusu saklama tutun](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Çözüm:**
    
  - RetentionHold ayarı belirli bir posta kutusu [EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)PowerShell'de durumunu denetleyin:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Belirli bir posta kutusuna RetentionHold **devre dışı bırakmak** için aşağıdaki komutu çalıştırın:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Şimdi, yönetilen Klasör Yardımcısı'nı yeniden çalıştırın:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Not:** Posta kutusu 10 MB'den küçükse, yönetilen Klasör Yardımcısı otomatik olarak posta kutusu işlemez.
 
Exchange Yönetim Merkezi'ndeki bekletme ilkeleri hakkında daha fazla bilgi için bkz:
- [Bekletme etiketler ve bekletme ilkeleri](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Posta kutularına bir bekletme ilkesi uygulayın](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Bekletme Etiketler Ekle Kaldır](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Ayrı tutma türünü tanımlamak nasıl bir posta kutusuna yerleştirilen](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
