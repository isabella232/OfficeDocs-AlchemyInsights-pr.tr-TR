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
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713666"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-postayı arşiv posta kutusuna taşıma

1. **Arşiv posta kutusunun** etkinleştirildiğini doğrulayın. Değilse, arşiv posta kutusunu etkinleştirmek için [bu makaledeki](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) adımları kullanın.

2. İletileri arşiv posta kutusuna otomatik olarak arşivlemek için, **arşive taşı** eylemini içeren bir bekletme **etiketinin tüm posta kutusu (varsayılan) etiketine otomatik olarak uygulanacak**şekilde ayarlanması gerekir. Etiketi oluşturmak için buradaki adımları kullanın: [Varsayılan etiketi ni arşivleyin.](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)

3. Ardından, bekletme ilkenize **Arşiv** etiketini ekleyin. Exchange yönetici merkezinde, **Bekletme İlkeleri'ni** seçin > **Kaydet**> ilkesine **Arşive Taşı etiketini** ekleyin.

4. Şimdi [Bekletme İlkesi'ni](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) belirli kullanıcının posta kutusuna atayın. Aynı ilke hem **Birincil** hem de **Arşiv** posta kutusuna uygulanır.

Yönetilen Klasör Yardımcısı'nı (MFA) yeni ayarları çalıştırmaya ve kullanıcının posta kutusuna uygulamaya zorlamak gerekebilir. Belirli bir posta kutusu için Yönetilen Klasör Yardımcısı'nı başlatmak için [EXO PowerShell'e bağlıyken](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) aşağıdaki komutu çalıştırın:
  
Başlat-YönetilenFolderAssistant -Kimlik<name of the mailbox>

Arşiv ilkesi ayarlama hakkında daha fazla bilgi için [bkz.](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  