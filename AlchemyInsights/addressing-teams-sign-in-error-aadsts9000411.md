---
title: Teams oturum açma hatasını ele aADSTS9000411
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
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822007"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Teams oturum açma hatasını ele aADSTS9000411

Microsoft Teams'de oturum aken şu hatayı alabilirsiniz: Üzgünüz, ancak AADSTS9000411'da oturum a açmayla ilgili sorun gidermeyle ilgili bir sorun oluştu: İstek düzgün **biçimlendir değil. "Login_hint" parametresi çoğaltıldı.**

Bu sorunu gidermek için lütfen Microsoft Teams istemcilerinizi güncelleştirilir. İstemcinizi güncelleştirme hakkında daha fazla bilgi için bkz. [Microsoft Teams'i güncelleştirme.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

İstemcinizi herhangi bir nedenden dolayı güncelleştire değilken, istemciyi kapatsanız önbelleğe alınan verilerin çoğunu temiz olur. Ancak logoff/oturum açma sonrasında da sorun yaşıyorsanız, Teams'den çıkın ve lütfen şunları yaparak istemci önbelleğinizi temizleyin:
1. Microsoft Teams'i kapatın.
2. %appdata%\microsoft\teams klasörüne gidin ve tüm dosyaları silin.
3. Microsoft Teams'i yeniden açın.
