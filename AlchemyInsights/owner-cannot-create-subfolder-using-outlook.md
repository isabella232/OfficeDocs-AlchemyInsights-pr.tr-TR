---
title: Sahip Outlook'u kullanarak alt klasör oluşturamaz
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836155"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Sahip Outlook'u kullanarak alt klasör oluşturamaz

**Ortak klasör sahiplerinin Outlook kullanarak alt klasör oluşturması sorunu devam ediyor. Sorun yakında giderilecek.**

Bu sırada, aşağıdaki geçici çözümlerden birini kullanın:

1. Alt klasörü oluşturmak için MAC için Outlook'u kullanın, bu sorun yalnızca Masaüstü için Outlook pencerelerini etkiler (tüm sürümler)
2. Yöneticinin EXO Shell veya EAC kullanarak alt klasör oluşturmasını
3. Kullanıcıda DefaultPublicFolderMailbox/EffectivePublicFolderMailbox'i, soruna neden olan klasörün İçerik Posta Kutusu'dan başka bir posta kutusuyla değiştirme  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Bir saat bekleyin, Outlook istemcisini yeniden başlatın