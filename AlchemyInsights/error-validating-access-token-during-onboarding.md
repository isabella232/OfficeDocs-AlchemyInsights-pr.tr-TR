---
title: Desktop Analytics'e kabul edilirken erişim belirteci hatasını doğrulama hatası oluştu
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813708"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Desktop Analytics ekleme sırasında "Erişim belirteci doğrulayla ilgili bir hata oluştu" hatası

Bu hata normalde kimlik doğrulama belirtecin süresi dolduğunda gözlemlenir. Genellikle, sayfa yenilendiğinde belirteci yeniler. Bununla birlikte, tahtada Desktop Analytics'e kullanılan hesaba uygulanmış herhangi bir Koşullu Erişim ilkesi varsa bu sorun kalıcı olabilir. Desktop Analytics ekleme için kullanılan hesapta herhangi bir oturum açma hatası olup kontrol etmek için Azure Portal'daki Azure AD Oturum Açma günlüklerini gözden geçirebilirsiniz.

Koşullu Erişim hakkında daha fazla bilgi için Koşullu Erişim [dağıtımınızı planlama .](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)