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
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816392"
---
# <a name="create-a-group"></a>Grup oluşturma

Bu konu başlığında grup oluşturma açıklanmıştır.

**Grup Oluşturma İzni**

Yeni grup oluşturma yetkinizin olduğundan emin olmak. Genel yöneticiler Azure portalda veya Erişim Masası'nda grup oluşturma özelliğini devre dışı bırakabilirsiniz. Sizin için yeni grup oluşturmak veya size uygun izinleri vermek için bir yöneticiye ihtiyacınız olabilir.

**Grup oluşturma izinlerini yönetme**

1. Genel yöneticiler, Tüm gruplar Genel   >  **(Ayarlar)** içinde "Kullanıcılar Azure portallarında güvenlik grupları oluşturabilir" veya "Kullanıcılar Azure portallarında Office 365 grupları oluşturabilir" seçeneklerini seçerek (güvenlikle ilgili nedenlerle) Azure portalında veya Erişim Paneli'de oluşturulan Office 365 gruplarını yönetebilir.
2. Azure Active Directory P1 Premium lisansınız varsa, grup oluşturma seçeneğini kısıtlayan bir kullanıcı grubu da kullanabilirsiniz.

**Yeni Office 365 grup üyeleri için karşılama bildirimini devre dışı bırakma**

Office 365 gruplarına eklenen kullanıcılara gönderilen karşılama bildirimi, Powershell'de **UnifiedGroupWelcomeMessageEnabled** değeri False olarak ayarlanabilir. Bu ayar hakkında buradan bilgi [öğrenebilirsiniz.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

