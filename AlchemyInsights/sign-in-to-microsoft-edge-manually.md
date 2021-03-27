---
title: Microsoft Edge'de el ile oturum açma
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398677"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Microsoft Edge'de el ile oturum açma

İlk çalıştırma deneyimi sırasında kullanıcı otomatik olarak oturum açmamışsa, kullanıcı tarayıcının ayarlarından veya kimlik açılır penceresinden el ile oturum açın. Oturum açmayı yönetmek için aşağıdaki ilkeleri kullanın:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - Kullanıcının Microsoft Edge'de her zaman iş profili olduğundan emin olmak için.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - Oturum açmayı güvenilir hesap kümesiyle kısıtlamak için.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - Oturum açma özelliğini devre dışı bırakmak veya kullanıcıları oturum açmaya zorlamak için.

