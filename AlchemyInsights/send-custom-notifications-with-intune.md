---
title: Intune ile özel bildirimler gönderme
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886877"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Yönetilen iOS ve Android cihazların kullanıcılarına özel bildirimler nasıl gönderilir?

Intune için özel bildirimler, Şirket Portalı uygulaması tarafından kullanıcının cihazında işlenir. Uygulama daha sonra bu cihazda anında iletme bildirimi oluşturur.

Özel bildirimlerin alınmasını desteklemek ve uygulamanın daha sonra anında iletme bildirimini oluşturması için cihaz ön koşulları şunlardır:

- Cihaz, Şirket Portalı uygulamasını yüklü olmalıdır.  

- Cihaz, Şirket Portalı uygulamasının anında iletme bildirimleri göndermesine izin vermelidir. Uygulama yüklendiğinde veya güncelleştirildiğinde, kullanıcıdan bildirimlere izin vermesini ister.

- Android cihazlarda Google Play Hizmetleri yüklü olmalıdır.

- Cihaz Intune ile kayıtlı olmalıdır.

İleti nin nasıl gönderilebildiğini de içeren daha fazla bilgi için [özellik belgelerine](https://docs.microsoft.com/intune/custom-notifications)bakın.
