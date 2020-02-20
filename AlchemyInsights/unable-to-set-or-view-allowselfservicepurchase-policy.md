---
title: AllowSelfServicePurchase ilkesini ayarlayamıyor veya görüntüleyemiyor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158581"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>AllowSelfServicePurchase ilkesini ayarlayamıyor veya görüntüleyemiyor

AllowSelfServicePurchase ilkesini ayarlamaya veya görüntülemeye çalışırken aşağıdaki hata iletisini alırsınız:

*HandleError : PolicyId 'AllowSelfServicePurchase' ile ürün ilkesi alınamadı, ErrorMessage - Altta yatan bağlantı kapatıldı: Gönderimde beklenmeyen bir hata oluştu.*

Bunun nedeni, Aktarım Katmanı Güvenliği'nin (TLS) eski bir sürümü olabilir. MSCommerce hizmetini bağlamak için TLS 1.2 veya daha büyük bir şekilde kullanmanız gerekir.  

TLS protokolünü etkinleştirmek/1,2 olarak ayarlamak, doğrulamak ve yeniden denemek için aşağıdaki adımları deneyin.
 1. PowerShell komut isteminde (PS\) C: TLS protokolünü sürüm 1.2'ye ayarlamak için aşağıdaki komutu girin:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Kullanımdaki TLS protokolünü aşağıdaki komutla doğrulayın:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Gerektiğinde Get or Update komutlarını yeniden deneyin.

