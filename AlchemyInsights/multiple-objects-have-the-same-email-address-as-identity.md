---
title: Birden çok nesne kimlikle aynı e-posta adresine sahiptir
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439707"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Birden çok nesne kimlikle aynı e-posta adresine sahiptir

**Birden çok nesne**

Bu hatanın yaygın nedenlerinden biri, kimlikle aynı e-posta adresine sahip birden çok nesnenin varlığında bir Outlook Web Access isteğini düzgün bir şekilde yönlendirememektir. Bu nesneleri bulmak için aşağıdaki komutları çalıştırın:

· Alıcı Al<email address>

· Kullanıcı Al<email address>

· Get-User <email address> -SoftDeletedUser

· İletişim Kurun<email address>

· Posta Kutusu Al <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

Sorunu gidermek için, aynı e-posta kimliğine sahip birden çok nesneyi kaldırın ve belirli e-posta kimliğine sahip tek bir nesne olduğundan ve alıcı türünün UserMailbox olduğundan emin olun.

**Aynı adres iş ve tüketici posta kutuları için kullanılır**

Başka bir nedeni aynı adres iş ve tüketici posta kutuları için kullanılır. Bu durumda, Cafe bu senaryoyu destekleyene kadar kullanıcının birincil tüketici takma adını değiştirmesi gerekir. Bu müdahale olmadan gitmez kalıcı bir hatadır.

Ayrıntılar için Microsoft [hesabınızın e-posta adresini veya telefon numarasını değiştir'e](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)bakın.