---
title: Klasik SharePoint denetim günlüğü raporları
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509620"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint ve OneDrive denetim günlükleri

## <a name="sharepoint-classic-audit-logs"></a>SharePoint klasik Denetim günlükleri

SPO eski denetimi Birleşik Denetim Günlüğü'ne (UAL) geçirildi. Tüm SPO eski denetim raporları artık UAL üzerinden desteklenecek ve eski denetim sinyalleri UAL'a geçirilmiştir.

Önemli değişiklikler:

* Kırpma bir yetenek olarak kullanılabilir DeğİlDir.
* Denetlemek için belirli olayları seçmek mevcut DeğİlDIR. Varsayılan olarak kullanılabilir denetlenen olayların tam listesi için [bu belgeye](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) bakın.
* **Özelleştirilmiş raporlar** altında **Konum** seçeneği kullanılabilir DeğİlDİr.
* **Belgeleri açma veya indirme** olayı seçeneği kullanılamıyor.

[Site koleksiyonu için Denetim ayarlarını yapılandırma](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Uyumluluktan SharePoint ve OneDrive Modern Birleşik Denetim günlükleri

* [Birleşik Denetim Günlüğe Kaydetme/Kapatma](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

SharePoint veya OneDrive içinde ek yapılandırma gerekmez.

Dosya(lar), klasör(ler), kullanıcı(lar), izinlerin etkinliğini denetlemek için denetim günlüğü aramasını kullanın:

* [Dosya ve sayfa etkinlikleri](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Klasör etkinlikleri](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [İstek etkinliklerini paylaşma ve erişim](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Senkronizasyon etkinlikleri](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Site yönetimi faaliyetleri](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Bu olayların nasıl alınabildiğini hakkında daha fazla bilgi için [denetim günlüğüne ara'ya](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)bakın.
