---
title: Cihazı Etkinleştir
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256988"
---
# <a name="enable-device"></a>Cihazı Etkinleştir

**Powershell komutunu kullanarak cihazı etkinleştirmek için**

Aşağıdaki komutları çalıştırın:

- Cihaz nesnesi almak için: `Get-MsolDevice -Name <Name>`
- Cihazı etkinleştirmek için: `Enable-MsolDevice -DeviceId <DeviceId>`

Yönetilen etki alanlarında Karma Birleştirmeyi Yapılandırma hakkında daha fazla bilgi için bkz. [Karma Birleştirmeyi Yapılandırma.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
