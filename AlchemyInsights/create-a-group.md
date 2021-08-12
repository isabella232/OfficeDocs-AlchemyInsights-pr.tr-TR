---
title: Grup oluşturma
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929325"
---
# <a name="create-a-group"></a>Grup oluşturma

Bu konu başlığında grup oluşturma açıklanmıştır.

**Grup Oluşturma İzni**

Yeni grup oluşturma yetkinizin olduğundan emin olmak. Genel yöneticiler Azure portalda veya Erişim Masası'nda grup oluşturma özelliğini devre dışı bırakabilirsiniz. Sizin için yeni grup oluşturmak veya size uygun izinleri vermek için bir yöneticiye ihtiyacınız olabilir.

**Grup oluşturma izinlerini yönetme**

1. Genel yöneticiler, Tüm gruplar Genel   >  **(Ayarlar)** seçeneğinde "Kullanıcılar Azure portallarında güvenlik grupları oluşturabilir" veya "Kullanıcılar Azure portallarında güvenlik grupları oluşturabilir" seçeneklerini seçerek (güvenlikle ilgili nedenlerle) grup oluşturma izinlerini veya Azure portallarında oluşturulmuş Office 365 Office 365 gruplarını yönetebilir.
2. Ayrıca, Azure Active Directory P1 lisansınız varsa, grup oluşturma Premium kısıtabilirsiniz.

**Yeni grup üyeleri için karşılama Office 365 devre dışı bırakma**

Office 365 gruplarına eklenen kullanıcılara gönderilen karşılama bildirimi, Powershell'de **UnifiedGroupWelcomeMessageEnabled** değeri False olarak ayarlanabilir. Bu ayar hakkında buradan bilgi [öğrenebilirsiniz.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

