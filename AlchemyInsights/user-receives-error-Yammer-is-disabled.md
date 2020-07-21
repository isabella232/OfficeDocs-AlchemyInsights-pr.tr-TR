---
title: Kullanıcı hata alır AADSTS7000112 Yammer devre dışı bırakılır
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198368"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Kullanıcı hata alır AADSTS7000112 Yammer devre dışı bırakılır

"AADSTS7000112: Application '0000000-0ff1-ce00-000000000000'(Yammer) devre dışı bırakılır" hatasını alırsanız, Azure AD içindeki hizmet müdüründe bir sorun vardır. Bir yönetici, Yammer'a erişimi engellemek için hizmet yöneticisini devre dışı bıraktı.

Hizmet ilkesini devre dışı bırakmak önerilmez ve ek sorunlara neden olabilir. Yammer kullanıcı erişimini engellemek için desteklenen yaklaşım hakkında daha fazla bilgi için [bkz.](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)  

Azure Portalı'ndaki bu sorunu düzeltmek ve Kullanıcı erişimini Yammer'a geri yüklemek için:

1.  Azure Etkin Dizin sayfasını açın ve sol gezinti bölmesinde **Yönet** altındaki **Kurumsal uygulamaları** seçin.
3.  Arama kutusuna **Office 365 Yammer** yazın ve ayarları açmak için uygulama adını seçin.
4.  Sol gezinti bölmesinde **Yönet** altındaki **Özellikleri** seçin.
5.  Kullanıcıların oturum **açmaları için Etkin'in** değerini evet **olarak**ayarlayın ve ardından **Kaydet'i**seçin.
6.  Yammer'la tekrar anlaş. Çerezleri temizlemeniz gerekebilir.

Alternatif olarak, değeri ayarlamak için PowerShell komutlarını çalıştırın. Daha fazla bilgi için, [Office 365'teki Yammer döşemesini tıklattığınızda "Üzgünüz, ancak oturum açmada sorun yaşıyoruz" hatasına](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)bakın. 