---
title: Teams başlat değil
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813361"
---
# <a name="teams-doesnt-launch"></a>Teams başlat değil

Bir dosyayı açmaya Microsoft Teams ama hiç açılmazsa, şunları deneyin:

1. **%appdata%\Microsoft\Teams klasörüne gidin.**
1. Klasörün içeriğini silin.
1. Bilgisayarı yeniden başlatın ve yeniden başlatmayı Teams.

E-Teams. Yeniden yüklemek için:

1. Denetim masası Teams denetimlerini kaldırın.
1. **%appdata%\Microsoft\Teams\Application Cache klasörüne gidin.**
1. Klasörün içeriğini silin.
1. **%appdata%\Microsoft\teams\Cache klasörüne göz atabilirsiniz.**
1. Klasörün içeriğini silin.
1. Bilgisayarı yeniden başlatın ve ardından yeniden Teams.

Kiracınız üzerinde oturum alıkan belirli bir kullanıcı için bir tanılama çalıştırmak için **TeamsUserUnableToSignIn** anahtar sözcüğüyle yeni bir arama çalıştırın ve istemleri izleyin.