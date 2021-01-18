---
title: VM 'Lere katılma sorunu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885658"
---
# <a name="issue-joining-vms"></a>VM 'Lere katılma sorunu

VM 'Lere katılmaya çalışırken oluşan sorunları çözmek için aşağıdaki adımları uygulayın:

1. **SAMAccountName** biçimi yerine **UPN** biçimini (örneğin, ' joeuser@contoso.com ') kullanarak oturum açmayı deneyin (' contoso\joeuser ').
2. *Başlarken* kılavuzunda anlatılan adımlara uygun olarak parola eşitlemesini etkinleştirdiğinizden emin olun.
3. Etkilenen Kullanıcı hesabının Azure AD kiracısında dış hesap olmadığından emin olun. Azure AD etki alanı Hizmetleri bu kullanıcı hesaplarının kimlik bilgilerini içermediğinden, dış kullanıcılar yönetilen etki alanında oturum açamaz.
4. Etkilenen Kullanıcı hesabı yalnızca bulut Kullanıcı hesabandır, Azure AD etki alanı Hizmetleri 'ni etkinleştirdikten sonra kullanıcıların parolasını değiştirmeyeceğinden emin olun. Bu adım, Azure AD etki alanı Hizmetleri için gereken kimlik bilgilerinin üretilmesine neden olur.
5. Etkilenen Kullanıcı hesapları şirket içi bir dizinden eşitleniyorsa, önerilen Azure AD Connect sürümünün tam eşitleme yapacak şekilde yapılandırılmış olduğunu doğrulayın.
6. Adım 4 ' ü onayladıktan sonra sorun devam ediyorsa, eşitleme makinenizden aşağıdaki komutları yürütün:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.