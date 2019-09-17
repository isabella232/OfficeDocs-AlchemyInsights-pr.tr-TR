---
title: Intune ile özel bildirimler gönderme
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992332"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Yönetilen iOS ve Android cihazların kullanıcılarına özel bildirimler nasıl gönderilir?

Intune için özel bildirimler, Şirket Portalı uygulaması tarafından kullanıcının cihazında işlenir. Uygulama daha sonra bu cihazda anında iletme bildirimi oluşturur.

Özel bildirimlerin alınmasını desteklemek ve uygulamanın daha sonra anında iletme bildirimini oluşturması için cihaz ön koşulları şunlardır:

- Cihaz, Şirket Portalı uygulamasını yüklü olmalıdır.  

- Cihaz, Şirket Portalı uygulamasının anında iletme bildirimleri göndermesine izin vermelidir. Uygulama yüklendiğinde veya güncelleştirildiğinde, kullanıcıdan bildirimlere izin vermesini ister.

- Android cihazlarda Google Play Hizmetleri yüklü olmalıdır.

- Cihaz Intune ile kayıtlı olmalıdır.

İleti nin nasıl gönderilebildiğini de içeren daha fazla bilgi için [özellik belgelerine](https://docs.microsoft.com/intune/custom-notifications)bakın.
