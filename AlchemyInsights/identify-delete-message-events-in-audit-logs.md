---
title: Denetim günlüklerinde ileti olaylarını silme'yi tanımlama
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716516"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Silinen e-posta iletileri için denetim günlükleri

Ocak 2019'dan itibaren Microsoft varsayılan olarak posta kutusu denetim günlüğe kaydetmeyi açıyor. Aksi takdirde, belirli bir kullanıcı için ileti olayları silme gözden geçirmek için, denetim için silme eylemleri el ile etkinleştirmek gerekir. Kuruluşunuz veya belirli bir kullanıcı için posta kutusu denetim günlüğü zaten etkinse, aşağıdaki adımları izleyin.

1. [Microsoft 365 Güvenlik & Uyumluluk Merkezi'nde](https://protection.office.com/) oturum açın

2. **Arama ve Araştırma'yı** tıklatın ve **Denetim Günlüğü Arama'yı**seçin.

3. **Başlangıç tarihi** ve Bitiş **tarihi** alanlarındaki tarih aralığını seçin. Araştırmak istediğiniz kullanıcı (öğeleri silen kullanıcı) için kullanıcı adı belirtin. **Etkinlikler** alanında, **Silinmiş Öğeler klasöründen Silinmiş iletileri** ve **Silinmiş Öğeler klasörüne taşınan iletileri**seçin.

4. **Arama'yı**tıklatın.

Sonuçlarda, bir denetim kaydı seçin. Ayrıntılarflyout, daha **fazla bilgi**tıklatın. Silinen öğe yle ilgili ek bilgiler (örneğin, konu satırı ve silindiğinde öğenin konumu) **Etkilenen Öğeler** alanında görüntülenir. **ClientInfoString** özelliği silme outlook, Outlook web (eski Outlook Web App olarak da bilinir) veya başka bir aygıtta oluştu gösterir.

Daha fazla bilgi için [bkz.](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)

**Not**: Denetim günlüğü özelliğini kullanarak silinen öğeleri alamazsınız. Web'de Outlook'ta silinen iletileri almak için [bkz.](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
