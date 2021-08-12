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
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946635"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Desktop Analytics ekleme sırasında "Erişim belirteci doğrulayla ilgili bir hata oluştu" hatası

Bu hata normalde kimlik doğrulama belirtecin süresi dolduğunda gözlemlenir. Genellikle, sayfa yenilendiğinde belirteci yeniler. Bununla birlikte, tahtada Desktop Analytics'e kullanılan hesaba uygulanmış herhangi bir Koşullu Erişim ilkesi varsa bu sorun kalıcı olabilir. Desktop Analytics ekleme için kullanılan hesapta herhangi bir oturum açma hatası olup kontrol etmek için Azure Portal'daki Azure AD Oturum Açma günlüklerini gözden geçirebilirsiniz.

Koşullu Erişim hakkında daha fazla bilgi için Koşullu Erişim [dağıtımınızı planlama .](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)