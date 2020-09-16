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
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange Yönetim merkezinde bekletme Ilkeleri

Aşağıda belirtilen ayarlar için otomatik denetimler 'in çalıştırılmasını istiyorsanız, bu sayfanın en üstündeki geri düğmesini < seçin ve ardından bekletme ilkeleriyle ilgili sorun olan kullanıcının e-posta adresini girin.

 **Sorun:** Exchange Yönetim merkezinde yeni oluşturulan veya güncelleştirilen bekletme ilkeleri posta kutularına veya öğeler arşiv posta kutusuna taşınmaz veya silinir. 
  
 **Kök nedenler:**
  
- Bu, **yönetilen klasör Yardımcısı 'nın** kullanıcının posta kutusunu işlemediği için olabilir. Yönetilen klasör Yardımcısı, bulut tabanlı kuruluşunuzdaki her posta kutusunu yedi günde bir kez işlemeye çalışır. Bir bekletme etiketini değiştirir veya posta kutusuna farklı bir bekletme ilkesi uygularsanız, yönetilen klasör Yardımcısı 'Nın posta kutusunu işlemesini bekleyebilirsiniz veya belirli bir posta kutusunu işlemek üzere yönetilen klasör Yardımcısı 'nı başlatmak için Start-ManagedFolderAssistant cmdlet 'ini çalıştırabilirsiniz. Bu cmdlet 'i çalıştırmak, bekletme ilkesi veya bekletme etiketi ayarlarını sınamak veya sorun gidermek için kullanışlıdır. Daha fazla bilgi için [yönetilen klasör Yardımcısı 'Nı çalıştırmayı](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)ziyaret edin.
    
  - **Çözüm:** Belirli bir posta kutusunun yönetilen klasör Yardımcısı 'nı başlatmak için aşağıdaki komutu çalıştırarak:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- **RetentionHold** , posta kutusunda **etkinleştirilmişse** da bu olabilir. Posta kutusu bir RetentionHold üzerine yerleştirilmişse, bu süre içinde posta kutusundaki bekletme ilkesi işlenmeyecektir. RetentionHold ayarında daha fazla bilgi için [bkz.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
    
    **Çözümlerden**
    
  - [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)'teki belirli bir posta kutusundaki RetentionHold ayarının durumunu denetleyin:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Belirli bir posta kutusunda RetentionHold **devre dışı bırakmak** için aşağıdaki komutu bırakın:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Şimdi, yönetilen klasör Yardımcısı 'nı yeniden çalıştırarak:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Not:** Posta kutusu 10 MB 'den küçükse, yönetilen klasör Yardımcısı posta kutusunu otomatik olarak işlemez.
 
Exchange Yönetim merkezinde bekletme ilkeleri hakkında daha fazla bilgi için bkz:
- [Bekletme etiketleri ve bekletme ilkeleri](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Posta kutularına bekletme ilkesi uygulama](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Bekletme etiketlerini ekleme veya kaldırma](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Posta kutusuna yerleştirilen bekletme türlerini tanımlama](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
