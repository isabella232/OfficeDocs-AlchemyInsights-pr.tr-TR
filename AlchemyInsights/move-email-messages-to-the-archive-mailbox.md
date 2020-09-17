---
title: E-posta iletilerini arşiv posta kutusuna taşıma
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799800"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-postayı arşiv posta kutusuna taşıma

Aşağıda belirtilen ayarlar için otomatik denetimler 'in çalıştırılmasını istiyorsanız, bu sayfanın en üstündeki geri düğmesini < seçin ve ardından e-postayı arşiv posta kutularına taşıma sorunlarını yaşayan kullanıcının e-posta adresini girin.

1. **Arşiv posta kutusunun** etkinleştirildiğini onaylayın. Yoksa, [Bu makaledeki](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) adımları kullanarak arşiv posta kutusunu etkinleştirin.

2. İletileri otomatik olarak arşiv posta kutusuna arşivlemek için, **arşive taşı** eylemine sahip bir bekletme etiketi, **posta kutusu (varsayılan) etiketine otomatik olarak uygulanacak**şekilde ayarlanmalıdır. Etiket: [Arşiv varsayılan etiketini](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)oluşturmak için buradaki adımları kullanın.

3. Ardından, **Arşiv** etiketini bekletme ilkeniz ekleyin. Exchange Yönetim merkezinde **bekletme ilkeleri** 'ni seçin > Kaydet **'e taşı etiketini** **Kaydet > kaydedin**.

4. Artık [bekletme ilkesini](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) belirli bir kullanıcının posta kutusuna atayın. Aynı ilke hem **birincil** hem de **Arşiv** posta kutusuna uygulanacaktır.

Yönetilen klasör Yardımcısı (MFA) çalıştırmak ve yeni ayarları kullanıcının posta kutusuna uygulamak gerekebilir. Belirli bir posta kutusunun yönetilen klasör Yardımcısı 'nı başlatmak için [EXO PowerShell 'e bağlıyken](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) aşağıdaki komutu çalıştırırsınız:
  
Başlangıç-ManagedFolderAssistant-kimlik <name of the mailbox>

Arşiv [ilkesi ayarlama hakkında](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)daha fazla bilgi için bkz.
  