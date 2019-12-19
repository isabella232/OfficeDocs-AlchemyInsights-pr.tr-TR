---
title: Masaüstü Analytics on-boarding sırasında erişim belirteç hatasını doğrulayan bir hata oluştu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741298"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Masaüstü Analytics onboarding sırasında "Erişim belirteci doğrulama hatası" hatası oluştu

Kimlik doğrulama belirteci süresi dolduğunda bu hata normalde gözlenir. Genellikle, sayfanın yenilenmesi belirteci yeniler. Ancak, yerleşik Masaüstü Analitiği için kullanılan hesaba uygulanan Koşullu Erişim ilkeleri varsa, bu sorun devam edebilir. Masaüstü Analitiği onboarding için kullanılan hesapiçin oturum açma hatası olup olmadığını görmek için Azure Portalı'ndaki Azure REKLAM Oturum Açma günlüğünü inceleyebilirsiniz.

Koşullu Erişim hakkında daha fazla bilgi [için, Koşullu Erişim dağıtımınızı planlayın'ı ziyaret edin.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)