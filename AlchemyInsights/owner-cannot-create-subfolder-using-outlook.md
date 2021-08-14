---
title: Sahip, E-posta klasörünü kullanarak alt Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063144"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Sahip, E-posta klasörünü kullanarak alt Outlook

**Ortak klasör sahiplerinin Paylaşılan Klasörler kullanarak alt klasör oluşturmalarında devam eden bir Outlook. Sorun yakında giderilecek.**

Bu sırada, aşağıdaki geçici çözümlerden birini kullanın:

1. Sorun Outlook masaüstü pencereleri (tüm sürümler) için Outlook bir alt klasör oluşturmak üzere MAC için Outlook'i kullanın
2. Yöneticinin EXO Shell veya EAC kullanarak alt klasör oluşturmasını
3. Kullanıcıda DefaultPublicFolderMailbox/EffectivePublicFolderMailbox'i, soruna neden olan klasörün İçerik Posta Kutusu'dan başka bir posta kutusuyla değiştirme  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Bir saat bekleyin, Outlook istemcisini yeniden başlatın