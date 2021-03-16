---
title: Bing'de Microsoft Arama için arka plan hizmetini kaldırma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816341"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Bing'de Microsoft Arama için arka plan hizmetini kaldırma

Bing'de Microsoft Arama'nın arka plan hizmetini kaldırmak için aşağıdaki çözümlerini deneyin:

1. Özgün arama alt yapısı ayarlarına geri dönmek için aşağıdaki işlemi yapın:

    a. **Bing'i varsayılan arama motorunuz olarak kullan [iki durumlu düğmeyi](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) kapatın.**

    b. [Microsoft 365 yönetim merkezine gidin](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) ve kuruluşta bulunan tüm kullanıcıları etkileyen ayarın temizlerini seçin.

2. Tek bir cihazdan arka plan hizmetini kaldırmak için aşağıdaki görevleri yapın:

    a. Programlar **ve Özellikler > Denetim > Seçin.**

    b. Yüklü programlar **listesinin altındaki Bing'de Microsoft** Arama'ya sağ tıklayın ve sonra Kaldır'a **tıklayın.**

3. Arka plan hizmetini kurumdaki birden çok cihazdan kaldırmak için, yönetici olarak oturum açın ve betikte aşağıdaki komutu çalıştırın: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
