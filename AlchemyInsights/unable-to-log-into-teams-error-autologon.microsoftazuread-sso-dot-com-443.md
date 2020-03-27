---
title: autologon.microsoftazuread-sso.com:443 Hatası nedeniyle Teams’te oturum açılamadı
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932285"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>autologon.microsoftazuread-sso dot com:443 Hatası nedeniyle Teams’te oturum açılamadı

O365 kimlik doğrulaması olarak Sorunsuz SSO etkinleştirildiyse, "autologon.microsoftazuread-sso.com URL’sinin Intranet Siteleri’ne eklenmesi gerelebilir.  Daha önce Güvenilen Siteler’e eklendiyse ve Sorunsuz SSO kullanılıyorsa, Güvenilen Siteler’den kaldırılmalıdır.

Lütfen [Sorunsuz SSO Sorun Giderme Denetim Listesi](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist) başlığını inceleyin.

Intranet Siteleri listesine URL eklemek için bu adımları izleyin:

1. **Başlat** düğmesine tıklayarak Internet Explorer’ı açın. Arama kutusuna Internet Explorer yazın ve sonuç listesinde **Internet Explorer**’a tıklayın.
2. **Araçlar**’a tıklayın ve ardından **İnternet seçenekleri**’ne tıklayın.
3. **Güvenlik** sekmesine tıklayın.
4. Şimdi, **Lerel Intranet Siteleri**’ne ve ardından **Siteler** düğmesine tıklayın ve sonra da **Gelişmiş** düğmesine tıklayın.
5. Web sitesi URL’sini girin ve **Ekle**’ye tıklayın.
6. Bitirdiğinizde **Kaydet**'e tıklayın.

Daha fazla bilgi edinmek için bkz. [O365 için Kesintisiz SSO’yu dağıtma Belgeleri](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (3. adımda Intranet Sitelerine bir URL eklemek için İlke tabanlı bir işlem içerir).
