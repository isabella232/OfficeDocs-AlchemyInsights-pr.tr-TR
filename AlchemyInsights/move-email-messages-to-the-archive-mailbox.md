---
title: Arşiv posta kutusuna e-posta iletileri taşı
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a29fb799b68f5c187ca1d44aeaf94e6cd8760b0e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35379517"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-posta arşiv posta kutusuna taşımak

1. Bir **posta kutusu arşiv** etkinleştirilmiş olduğunu doğrulayın. Tersi durumda, arşiv posta kutusunu etkinleştirmek için [Bu makalede](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) adımları kullanın.

2. Otomatik Arşiv posta iletilerini arşivlemek için **arşive Taşı** eylemini içeren bir bekletme etiket **otomatik olarak tüm posta kutusu (varsayılan) imine verilen**ayarlanması gerekir. Buraya etiket oluşturmak için adımları kullanın: [Arşiv varsayılan etiket](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).

3. Sonra **Arşiv** etiketi, bekletme ilkesine ekleyin. Exchange Yönetim Merkezi'nde **Bekletme ilkeleri** seçin > eklemek **taşımak için etiket arşiv** İlkesi > için **Kaydet**.

4. Şimdi [bekletme ilkesini atamak](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) için belirli bir kullanıcının posta kutusu. Hem **birincil** hem de **Arşiv** posta kutusu için aynı ilke uygulanacaktır.

Yönetilen Klasör Yardımcısı (çalıştırmak ve kullanıcının posta kutusu için yeni ayarları uygulamak için MFA) zorlamak gerekli olabilir. Yönetilen Klasör Yardımcısı belirli bir posta kutusu için başlatmak için [EXO PowerShell için bağlı](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) çalışırken aşağıdaki komutu çalıştırın:
  
Start-ManagedFolderAssistant-kimlik<name of the mailbox>

Arşiv İlkesi ayarlama hakkında daha fazla bilgi için bkz: [posta kutuları için bir arşiv ve silme ilkesi ayarlayın](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  