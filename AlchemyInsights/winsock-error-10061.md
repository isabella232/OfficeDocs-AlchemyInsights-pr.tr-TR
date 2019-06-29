---
title: 1554 Winsock hata 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e82e90b670235848105636fb2039ed60d3b93c67
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364933"
---
# <a name="winsock-error-10061"></a>WINSOCK Hatası: 10061

Bu hata kodunu Office 365 (bağlantı) ile hedef ana bilgisayarı bir TCP Yuvasını kurmak uygulanamadı anlamına gelir. Bu hatanın en olası nedeni, güvenlik duvarı yapılandırması ile ilgili bir sorun var. Sorunu gidermek için bu ayarları denetleyin:

- Bilgileri [Office 365 URL'leri ve IP adres aralıkları](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) ile güvenlik duvarı yapılandırmanızı doğrulayın

- Hata Exchange çevrimiçi koruma (EOP) belirli ise, daha önce bir değişiklik [Exchange çevrimiçi koruma IP adresleri](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)için bildirildi.

- Internet servis sağlayıcınıza (ISS) bağlantı noktası engellemediğinden emin olun.

- Bağlayıcılar, akıllı ana bilgisayar ve hedef sunucu ayarlarını doğrulayın.

Not Bu yolla *gelen* bağlantıları Office 365 engellemez.
