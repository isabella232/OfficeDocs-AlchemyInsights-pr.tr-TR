---
title: Teams için bir eklenti
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940695"
---
# <a name="teams-add-in-for-mac"></a>Teams için bir eklenti

Mac işletim sistemi Teams eksik hatayla ilgili sorunları gidermek için şu adımları izleyin:

**1. Adım:** Karma Kimlik Exchange Şirket İçi (2016 CU3 veya sonrası gerekli) kullanıyorsanız, Karma Modern Kimlik Doğrulaması'nın doğru yapılandırıldığından emin olmak için Test-HMA.ps1 aracını kullanın. Daha fazla bilgi için [bkz. iOS](https://aka.ms/TestHMAEAS)ve Android için Outlook Karma Modern Kimlik Doğrulama kurulumu doğrulama.  

**Not** ETKIalanı\kullanıcıadı değil UPN [adres biçimini (örneğin, username@contoso.com)](mailto:username@contoso.com)kullanın. Bu, e-posta kutusu Exchange Online alın.

**2. Adım:** Kullanıcının Araçlar Hesapları   >  ... oturum Mac için Outlook hesabı bulup seçin. Listelenen kullanıcı adlarının UPN biçiminde olduğunu [](mailto:username@contoso.com)onaylayın (örneğin, username@contoso.com).

**3. Adım:** Kullanıcının lisanslı bir kullanıcı olduğunu Microsoft Teams onaylayın. Kullanıcının Mac için Office 365, ürün sürümü 16.24 veya sonraki bir sürümünü kullanıyor olması gerekir.