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
ms.openlocfilehash: d0ef27e7c03eb8bcd9de74c58a5e0398d8892a6eb0ab50944b3c2201247fa0b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889238"
---
# <a name="active-directory-not-syncing"></a>Active Directory eşitli değil

"Yakın zamanda eşitleme yok" gibi eşitleme hataları alıyorsanız veya Office yönetim portalında dizin eşitleme durumunun "Son eşitleme 3 gün önce" olarak açıklanmış olduğunu fark ederseniz, AADConnect'in eşitlemeyi gerçekleştirmek için yanlış ayarlara veya yetersiz izinlere sahip olması olabilir.  

Hızlı ayarları kullanarak AADConnect'in yeniden yüklenmesi sorunu hızla çözebilir:

1. [AADConnect'in en son sürümünü indirin.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Hızlı yükleme yönergelerini izleyin.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect, Windows Server 2012 veya sonraki sürümlerde yüklü olmalıdır. Etki alanına katılmış olması gereken bu sunucu, etki alanı denetleyicisi veya üye sunucu olabilir. Azure AD Abonelik Gereksinimleri'nin Bağlan önkoşullarının tam listesi için Azure [AD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)Önkoşulları'Bağlan.

AADConnect hizmet hesapları hakkında daha fazla bilgi için bkz. [Azure AD Bağlan: Hesaplar ve izinler.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
