---
title: Sahip, Outlook kullanarak alt klasör oluşturamaz
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665738"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Sahip, Outlook kullanarak alt klasör oluşturamaz

**Outlook kullanan ortak klasör sahiplerinin alt klasörlerini oluşturmakla ilgili bir sorun var. Sorun yakında düzeltilecektir.**

Bu arada, aşağıdaki geçici çözümlerden birini kullanın:

1. MAC için Outlook 'U kullanarak sorun yalnızca masaüstü Windows için Outlook 'U (tüm sürümler) etkilediğdeyken alt klasörü oluşturmak için
2. EXO kabuğu veya EAC kullanarak alt klasörü oluşturma
3. Kullanıcıya, soruna neden olan klasördeki DefaultPublicFolderMailbox/Efekt\tüm  
    - *Set-Mailbox Kullanıcı1 DefaultPublicFolderMailbox PubMBX3*
4. Saat bekle, Outlook istemcisini yeniden başlatın