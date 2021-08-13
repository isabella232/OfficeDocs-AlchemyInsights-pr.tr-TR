---
title: E-posta iletilerini Arşiv posta kutusuna taşıma
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
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974977"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-postayı arşiv posta kutusuna taşıma

Aşağıda sözü geçen ayarlar için otomatik denetimleri çalıştırmamızı istemiyorsanız, bu sayfanın en üstünde yer alan geri düğmesini < seçin ve ardından e-postayı arşiv posta kutusuna taşımada sorun yaşanan kullanıcının e-posta adresini girin.

1. Arşiv posta kutusunun **etkinleştirildiğinden** emin olun. Yoksa, arşiv posta kutusunu [etkinleştirmek için bu](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) makaledeki adımları kullanın.

2. İletileri otomatik olarak arşiv posta kutusuna arşivlemek için, Arşive taşı eylemini bulunduran bir bekletme etiketinin, posta kutusu (varsayılan) etiketinin tamamına otomatik olarak  **uygulanıyor olması gerekir.** Etiketi oluşturmak için buradaki adımları kullanın: [Arşiv Varsayılan etiketi](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Ardından Arşiv etiketini **bekletme** ilkenize ekleyin. Exchange merkezinde Bekletme İlkeleri'ni **>** Kaydet'>  **ekleyin.**

4. Şimdi [Bekletme İlkesi'i](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) belirli bir kullanıcının posta kutusuna attayabilirsiniz. Aynı ilke hem Birincil hem de Arşiv **posta** **kutusuna** uygulanır.

Yönetilen Klasör Yardımcısı'nın (MFA) yeni ayarları kullanıcının posta kutusuna çalıştırması ve bu ayarları uygulaması için zorlamanız gerekebilir. Belirli bir posta kutusunun Yönetilen [Klasör Yardımcısı'na başlamak](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) için EXO PowerShell'e bağlıyken aşağıdaki komutu çalıştırın:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Arşiv ilkesi ayarlama hakkında daha fazla bilgi için [bkz. Posta kutuları için arşivleme ve silme ilkesi ayarlama](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  