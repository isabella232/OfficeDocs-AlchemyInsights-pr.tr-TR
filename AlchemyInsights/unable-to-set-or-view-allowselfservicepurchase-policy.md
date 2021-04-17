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
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826111"
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

