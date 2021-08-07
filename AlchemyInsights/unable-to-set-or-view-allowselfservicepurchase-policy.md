---
title: AllowSelfServicePurchase ilkesi ayarlanamıyor veya görüntüden silinemiyor
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
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020212"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>AllowSelfServicePurchase ilkesi ayarlanamıyor veya görüntüden silinemiyor

AllowSelfServicePurchase ilkesi ayarlamaya veya görüntülemeye çalışırken, aşağıdaki hata iletisini alısınız:

*HandleError: PolicyId 'AllowSelfServicePurchase', ErrorMessage ile ürün ilkesi alınamadı - Temel bağlantı kapatıldı: Gönderme sırasında beklenmeyen bir hata oluştu.*

Bunun nedeni Aktarım Katmanı Güvenliği'nin (TLS) eski bir sürümü olabilir. MSCommerce hizmetine bağlanmak için TLS 1.2 veya daha yeni bir değer kullan gerekir.  

TLS protokolünü 1,2 olarak etkinleştirmek/ayarlamak, doğrulamak ve yeniden denemek için aşağıdaki adımları deneyin.
 1. PowerShell komut isteminde (PS C: TLS protokolünü sürüm 1.2 olarak ayarlamak için \) aşağıdaki komutu girin:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Kullanımda OLAN TLS protokollerini şu komutu kullanarak doğrulayın:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Al veya Güncelleştir komutlarını gerektiğinde yeniden deneyin.

