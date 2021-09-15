---
title: Microsoft 365 yönetim merkezinde raporlar okunur bir kullanıcı adı göstermiyor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327834"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Microsoft 365 yönetim merkezinde raporlar okunur bir kullanıcı adı göstermiyor

Microsoft 365 yönetim merkezinde raporlar kullanıcı adlarını değil, bunun yerine B2BC6C15BB9FCDEA71E5CD302D228CC8 gibi alfanümerik değerler gösteriyor.

Bu beklenen bir davranıştır ve İleti Merkezi'nde iletilmiştir (MC275344, 3 Ağustos 2021’de yayımlandı). 

Genel yöneticiler, kiracıları için bu değişikliği geri alabilir ve kuruluş gizlilik uygulamaları izin veriyorsa tanımlanabilecek kullanıcı bilgilerini gösterebilir. Kiracı değişikliğini geri almak için:

1. Yönetim merkezinde, **Ayarlar** > **Kuruluş ayarları** > [**Hizmetler**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) ve **Raporlar**’a gidin. 
1. **Kullanıcı bilgilerini gösterme** öğesinin altında **Raporlarda tanınabilir kullanıcı bilgilerini göster** öğesini seçin ve raporu yeniden çalıştırın.