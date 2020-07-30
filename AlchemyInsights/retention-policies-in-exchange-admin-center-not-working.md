---
title: Exchange Yönetici Merkezi'nde Bekletme İlkeleri çalışmıyor
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522827"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange Yönetici Merkezinde Bekletme İlkeleri

Aşağıda belirtilen ayarlar için otomatik denetimler yapmamızı istiyorsanız, bu sayfanın üst kısmındaki < arka düğmesini seçin ve ardından bekletme ilkeleriyle ilgili sorunları olan kullanıcının e-posta adresini girin.

 **Sorun:** Exchange Yönetici Merkezi'nde yeni oluşturulan veya güncelleştirilen bekletme ilkeleri posta kutularına uygulanmaz veya öğeler arşiv posta kutusuna taşınmaz veya silinmez. 
  
 **Kök Nedenleri:**
  
- Bunun **nedeni, Yönetilen Klasör Yardımcısı'nın** kullanıcının posta kutusunu işlememiş olması olabilir. Yönetilen Klasör Yardımcısı, bulut tabanlı kuruluşunuzdaki her posta kutusunu yedi günde bir işlemeye çalışır. Bekletme etiketini değiştirir veya bir posta kutusuna farklı bir bekletme ilkesi uygularsanız, Yönetilen Klasör Yardımcısı'nın posta kutusunu işlemesini bekleyebilir veya belirli bir posta kutusunu işlemek için Yönetilen Klasör Yardımcısı'nı başlatmak için Başlat Yönetilen Klasör Yardımcısı cmdlet'ini çalıştırabilirsiniz. Bu cmdlet'i çalıştırmak, bekletme ilkesi veya bekletme etiketi ayarlarını sınamak veya sorun gidermek için yararlıdır. Daha fazla bilgi için Yönetilen Klasör Yardımcısını Çalıştır'ı ziyaret [edin.](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)
    
  - **Çözüm:** Belirli bir posta kutusu için Yönetilen Klasör Yardımcısı'nı başlatmak için aşağıdaki komutu çalıştırın:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- **Bu,** posta kutusunda Beklet **etkinleştirilmişse** de oluşabilir. Posta kutusu Bekletme Ambarı'na yerleştirilmişse, posta kutusundaki bekletme ilkesi bu süre içinde işleme alınmaz. Bekletme ayarında daha fazla bilgilendirme için bkz: [Posta Kutusu Bekletme .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
    
    **Çözüm:**
    
  - [EXO powershell'deki](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)belirli posta kutusundaki Bekletme Ayarı'nın durumunu denetleyin:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Belirli bir posta kutusunda Beklet'i **devre dışı kıtırmak** için aşağıdaki komutu çalıştırın:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Şimdi, Yönetilen klasör Yardımcısı yeniden çalıştırın:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Not:** Bir posta kutusu 10 MB'dan küçükse, Yönetilen Klasör Yardımcısı posta kutusunu otomatik olarak işlemez.
 
Exchange Yönetici Merkezi'ndeki bekletme ilkeleri hakkında daha fazla bilgi için bkz:
- [Bekletme etiketleri ve bekletme ilkeleri](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Posta kutularına bekletme ilkesi uygulama](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Bekletme etiketleri ekleme veya kaldırma](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Posta kutusuna yerleştirilen bekleme türünü belirleme](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
