---
title: Arşiv posta kutusuna e-posta iletileri taşı
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 2147c70f64087bf95fc4e39c193caeac3b2c5361
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660403"
---
Arşivleme işlemi öğeleri arşiv posta sorunlarınız. Aşağıdaki adımları gerçekleştirdiğiniz emin olun:
  
1. Bir **posta kutusu arşiv** etkinleştirilmiş olduğunu doğrulayın. Tersi durumda, arşiv posta kutusunu etkinleştirmek için [Bu makalede](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) adımları kullanın. 
    
2. Exchange Yönetim Merkezi'ndeki **Uyumluluk Yönetimi**altında **Tutma etiketleri** seçin, **arşive Taşı** eylemini istenen **Bekletme yaş**içeren bir **bekletme etiketi** oluşturmak.
    
3. Exchange Yönetim Merkezi, **Bekletme ilkeleri**seçin, bir **Bekletme ilkesi** oluşturun ve **arşive Taşı** bekletme etiketinizi bu ilkeye eklemek. 
    
4. [Bekletme ilkesini atamak](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) için belirli bir kullanıcının posta kutusu. Hem **birincil** hem de **Arşiv** posta kutusu için aynı ilke uygulanacaktır. 
    
Kullanıcının posta kutusu şimdi öğeleri arşiv posta kutusuna taşımak için bir Arşiv İlkesi olmalıdır. Yönetilen Klasör Yardımcısı (çalıştırmak ve kullanıcının posta kutusu için yeni ayarları uygulamak için MFA) zorlamak gerekli olabilir. Yönetilen Klasör Yardımcısı belirli bir posta kutusu için başlatmak için [EXO PowerShell için bağlı](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) çalışırken aşağıdaki komutu çalıştırın: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Bir Arşiv İlkesi hakkında daha fazla bilgi istiyorsanız, [posta kutuları için bir arşiv ve silme ilkesini ayarlama](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)konusuna bakın.
  

