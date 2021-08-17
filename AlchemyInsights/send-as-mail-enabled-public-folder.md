---
title: EXO'da Posta Etkin Olarak Gönder Ortak Klasör
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052586"
---
# <a name="sendas-mail-enabled-public-folder"></a>SendAs Mail Enabled Public Folder

Aşağıdaki örnekte, kullanıcı Jason'a posta özelliği etkin ortak klasör NewPF1 için "Farklı Gönder" izinleri atanıyor.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'

Ayrıntılı söz dizimi ve parametre bilgileri için bkz. Posta özellikli ortak klasörler için ["Farklı Gönder" veya "Adına Gönderme" izinleri.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)

