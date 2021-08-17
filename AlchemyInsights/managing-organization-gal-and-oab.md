---
title: Kuruluşun genel adres listesini ve çevrimdışı adres defterini yönetme
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
- "9002895"
- "5550"
ms.openlocfilehash: c5b73e2dae4d2b98b6af05e147f93a493bac5a88cfcb9ea67c979264aba34ceb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54042182"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>Kuruluşun genel adres listesini (GAL) ve çevrimdışı adres defterini (OAB) yönetme

Genel adres listesi (GAL) kuruluşta posta özellikli nesnelerin (e-posta alabilen her tür alıcı) listesidir. Her kuruluşta bir GAL otomatik olarak oluşturulur. Kullanıcıları kuruluşa veya konuma göre ayırmak için ek GAL’ler oluşturabilirsiniz ama bir kullanıcı aynı anda tek bir GAL görebilir ve kullanabilir.

Windows için Outlook gibi bazı e-posta istemcileri GAL’yi çevrimdışı kullanım için indirir. Bu, çevrimdışı adres defteri (OAB) olarak bilinir. Exchange Online’da OAB ancak 8 saatte bir güncelleştirilir ve bundan sonra istemcilerin yerel OAB kopyalarını güncelleştirmek için OAB’yi indirmeleri gerekir. Tüm alıcı değişikliklerinin OAB’ye geçmeden önce GAL’de görünür olması gerekir.

Aşağıda yaygın kullanılan bazı GAL ve OAB yordamları verilmiştir:

- Çeşitli nedenlerle bazı nesnelerin GAL’de gizlenmesini isteyebilirsiniz. Bkz. [Alıcıları adres listesinde gizleme](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).
- Belirli kullanıcı gruplarına kuruluşun GAL’sinin özelleştirilmiş görünümlerini vermeniz gerekirse bkz. [Exchange Online’da adres defteri ilkeleri](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).
- [Exchange Online’da genel adres listesi oluşturun](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) ve GAL izinleriyle çalışmayı öğrenmek için [Exchange Online’da adres listeleri](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists) konusuna bakın. Yeni GAL’ler oluşturursanız, yeni bir OAB de oluşturmak isteyebileceğinizi aklınızda bulundurun. Bkz. [Çevrimdışı adres defteri yordamları](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).
