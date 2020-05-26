---
title: Adresleme Takımlar oturum açma hatası AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358366"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Adresleme Takımlar oturum açma hatası AADSTS9000411

Microsoft Teams'de oturum açtığınızda hata alabilirsiniz: **Üzgünüz, ancak AADSTS9000411'de imzalamanızda sorun yaşıyoruz: İstek düzgün biçimlendirilmemiştir. "login_hint" parametresi çoğaltılır.**

Bu sorunu gidermek için lütfen Microsoft Teams istemcilerinizin güncelleştirdiğinden emin olun. İstemcinizi güncelleştirme hakkında daha fazla bilgi için Microsoft [Ekiplerini Güncelleştir'e](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)bakın.

İstemcinizi bir nedenle güncelleştiremiyorsanız, istemcinin oturumu kapatılır, önbelleğe alınan çoğu veriyi temizler. Ancak, oturum kapatma/oturum açma sonrasında hala sorunlarınız varsa, Takımlar'dan çıkın ve lütfen aşağıdakileri yaparak istemci önbelleğinizi temizleyin:
1. Microsoft Ekiplerini kapatın.
2. Şuna gidin: %appdata%\microsoft\teams ve tüm dosyaları silin.
3. Microsoft Ekiplerini yeniden açın.
