---
title: Varsayılan Outlook etiketi ayarı uygulanmadı
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/17/2021
ms.locfileid: "58455083"
---
# <a name="default-outlook-label-setting-not-applied"></a>Varsayılan Outlook etiketi ayarı uygulanmadı

Outlook varsayılan etiket ayarlarınız düzgün uygulanıyorsa ve farklı bir etiket uygulanmazsa veya etiket uygulanmazsa, bilinen bir sorun (MC277818) yaşıyor olabilir ve sorunu çözmek için şu 2 seçenekden birini yapmanız gerekir:

**1. Seçenek:**

1. Uyumluluk Merkezi Microsoft 365 Çözüm >   >  **Koruma'ya gidin.**
1. Etiket **ilkeleri'ne** tıklayın ve düzenlemeniz gereken etiket ilkesine tıklayın **(OutlookDefaultlabel** ayarı söz konusu etiket ilkesine düzgün ayarlanmaz. Bu **ayarı görüntülemek için Get-labelpolicy** seçeneğini çalıştırın ve sonra İlkeyi **düzenle'yi seçin.**
1. İlke ayarları iletişim kutusunda E-postalara bu varsayılan etiketi  uygula ayarını görene kadar Sonraki'yi seçin. Bu, İlke ayarları iletişim kutusunda Var olan e-postalara ve belgelere kullanıcıların etiket uygulamalarını gerektir seçeneğini görüyorsanız kullanılabilir.  
1. Belgelere **varsayılan etiket uygula iletişim** kutusunda, açılan listeden **Yok'a** tıklayın.
1. Etiket **ayarlarınızı kaydetmek** için **Sonraki** ve Gönder'i seçin.

**2. Seçenek:**

Güvenlik ve Uyumluluk Merkezi [Powershell'de](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)Set-LabelPolicy komutunu kullanarak **OutlookDefaultlabel** öğesini {OutlookDefaultLabel="None"} üzerinde **Yok** olarak değiştirebilirsiniz.

Çalıştır: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Posta etiketlerinin varsayılan etiketleri hakkında daha fazla Outlook için bkz. [Outlook.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)