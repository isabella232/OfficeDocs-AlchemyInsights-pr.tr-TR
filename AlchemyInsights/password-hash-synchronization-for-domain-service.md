---
title: Etki alanı hizmeti için parola karması eşitlemesi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177618"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Etki alanı hizmeti için parola karması eşitlemesi

**Azure AD DS örneğiniz parola karma eşitlemesini etkinleştirmenizi istendiğinde**

Karma bir ortamı, şirket içi Azure Active Directory Etki Alanı Hizmetleri (AD DS) ortamından eşitleen kullanıcılarla çalıştırıyorsanız, bir senaryoyla karşılaşırsınız. Şirket içi AD DS'den Azure AD kiracınıza parola karma eşitlemesi olmasına rağmen bu senaryoyla karşılaşıldı.

**Neden**

Bunun nedeni Azure AD Connect'in varsayılan olarak Azure AD DS için gereken eski Yeni Teknoloji LAN Manager (NTLM) ve Kerberos parola karmalarını eşitlememasıdır.

**Geçici Çözüm** 

NTLM ve Kerberos kimlik doğrulaması için gereken parola karmalarını eşitlemek için Azure AD Connect'i yapılandırmanız gerekir.

Azure AD Connect yapılandırıldığında, şirket içi hesap oluşturma veya parola değiştirme olayı da eski parola karmalarını Azure AD'ye eşitler. Bu işlem [hakkında](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) daha fazla bilgi ve Azure AD DS karma ortamlarında parola eşitlemesini etkinleştirme hakkında yol gösterici bilgiler için lütfen buraya bakın.