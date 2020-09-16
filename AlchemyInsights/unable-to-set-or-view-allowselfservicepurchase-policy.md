---
title: AllowSelfServicePurchase ilkesi ayarlanamıyor veya gösterilemiyor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735219"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>AllowSelfServicePurchase ilkesi ayarlanamıyor veya gösterilemiyor

AllowSelfServicePurchase ilkesini ayarlamaya veya görüntülemeye çalışırken aşağıdaki hata iletisini alırsınız:

*HandleError: PolicyId ' AllowSelfServicePurchase ' ile ürün ilkesi alınamadı, ErrorMessage-temeldeki bağlantı kapatıldı: gönderme sırasında beklenmeyen bir hata oluştu.*

Bu, taşıma katmanı güvenliğinin (TLS) eski bir sürümü olabilir. MSCommerce hizmetini bağlamak için, TLS 1,2 veya üzerini kullanmanız gerekir.  

TLS protokolünü 1,2, doğrulama ve yeniden deneyin.
 1. PowerShell komut isteminde (PS C: \) TLS protokolünü sürüm 1,2 olarak ayarlamak için aşağıdaki komutu girin:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Aşağıdaki komutla, kullanımdaki TLS protokollerini doğrulayın:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Gerektiğinde Al veya Güncelleştir komutlarını yeniden deneyin.

