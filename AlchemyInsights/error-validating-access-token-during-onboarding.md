---
title: Masaüstü analizi sırasında erişim belirteci hatası doğrulanırken hata oluştu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783571"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Masaüstü analitik ekleme sırasında "erişim belirteci doğrulanırken hata oluştu" hatası

Bu hata normalde kimlik doğrulama belirtecinin süresi dolduğunda izlenir. Genellikle, sayfayı yenilemek belirteci yeniler. Ancak, yerleşik masaüstü analizinde kullanılan hesaba herhangi bir koşullu erişim ilkesi uygulanmışsa bu sorun devam edebilir. Masaüstü Analizi ekleme için kullanılan hesabın oturum açma hataları olup olmadığını görmek için Azure portalında Azure AD oturum açma günlüklerini gözden geçirebilirsiniz.

Koşullu erişim hakkında daha fazla bilgi için [koşullu erişim dağıtımınızı planlayın](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)sayfasını ziyaret edin.