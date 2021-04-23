---
title: Exchange Yönetim Merkezi'nde Bekletme İlkeleri çalışmıyor
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952248"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange Yönetim Merkezi'nde Bekletme İlkeleri

Aşağıda adı geçen ayarlar için otomatik denetimleri çalıştırmamızı istemiyorsanız, bu sayfanın en üstünde yer alan geri düğmesini < seçin ve ardından bekletme ilkeleriyle ilgili sorunları olan kullanıcının e-posta adresini girin.

Exchange Yönetim Merkezi'nde bekletme ilkeleri posta kutularına veya arşiv posta kutusuna taşınmıyor olan öğelere uygulanmıyorsa, bekletme ilkeleriyle ilgili sorunlarınız varsa, şunları kontrol edin:

**Kök Nedenler:**

- **Yönetilen Klasör Yardımcısı** kullanıcının posta kutusunu işlemedi. Yönetilen Klasör Yardımcısı, bulut tabanlı kuruluşta her posta kutusunu yedi günde bir işlemeyi çalışır.

  **Çözüm:** Yönetilen Klasör Yardımcısı'nın çalıştırın.

- **Posta kutusunda RetentionHold** **etkinleştirildi.** Posta kutusu bir RetentionHold'a yerleştirilmişse, posta kutusunda bekletme ilkesi bu süre boyunca işlenmez.

  **Çözüm:** Bekletme Bekletme ayarının durumunu denetleme ve gerektiğinde güncelleştirme. Ayrıntılar için bkz. Posta [Kutusu Bekletme.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Not:** Posta kutusu 10 MB'den küçükse, Yönetilen Klasör Yardımcısı posta kutusunu otomatik olarak işlemez.
 
Exchange Yönetim Merkezi'nde bekletme ilkeleri hakkında daha fazla bilgi için bkz:

- [Bekletme etiketleri ve bekletme ilkeleri](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Posta kutularına bekletme ilkesi uygulama veya](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) Bekletme etiketleri ekleme veya [kaldırma](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Posta kutusuna yerleştirilen tutma türünü belirleme](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
