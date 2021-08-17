---
title: Active Directory eşitli değil
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314224"
---
# <a name="active-directory-not-syncing"></a>Active Directory eşitli değil

"Yakın zamanda eşitleme yok" gibi eşitleme hataları alıyorsanız ya da Office yönetim portalında dizin eşitleme durumunun "Son eşitleme 3 gün önce" olarak açıklanmış olduğunu fark ederseniz, AADConnect'in yanlış ayarları veya eşitlemeyi gerçekleştirmek için yetersiz izinleri olabilir.  

Hızlı ayarları kullanarak AADConnect'in yeniden yüklenmesi sorunu hızla çözebilir:

1. [AADConnect'in en son sürümünü indirin.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Hızlı yükleme yönergelerini izleyin.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect, Windows Server 2012 veya sonraki sürümlerde yüklü olmalıdır. Etki alanına katılmış olması gereken bu sunucu, etki alanı denetleyicisi veya üye sunucu olabilir. Azure AD Abonelik Gereksinimleri ve önkoşulların Bağlan listesi için Azure [AD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)Önkoşulları'Bağlan.

AADConnect hizmet hesapları hakkında daha fazla bilgi için bkz. [Azure AD Bağlan: Hesaplar ve izinler.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
