---
title: Outlook'u kullanarak ortak klasörlere erişimi denetleme
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816760"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Outlook'u kullanarak ortak klasörlere erişimi denetleme

Outlook'u kullanarak ortak klasörlere hangi kullanıcıların eriş erişeni kontrol etmek için:

1. Kullanım `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Kullanıcıların Outlook'ta ortak klasörlere erişmesine izin verme  
$false: Outlook'ta kullanıcının ortak klasörlere erişimini engelin. Bu, varsayılan değerdir.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Not: Bu yordam yalnızca Windows istemcileri için Outlook masaüstü ile bağlantıları kontrol eder. Kullanıcılar ortak klasörlere OWA veya Mac için Outlook'u kullanarak erişmeye devam ediyor.

Daha fazla bilgi için bkz. [Outlook'ta Ortak Klasörlere Denetimli](https://aka.ms/controlpf) Bağlantılar.
