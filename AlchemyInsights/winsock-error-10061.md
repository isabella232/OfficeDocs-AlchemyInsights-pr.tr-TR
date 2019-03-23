---
title: 1554 Winsock hata 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f44ed42906b85e63f1f694813f54710906969904
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30772461"
---
# <a name="winsock-error-10061"></a>WINSOCK Hatası: 10061

Bu hata kodunu Office 365 (bağlantı) ile hedef ana bilgisayarı bir TCP Yuvasını kurmak uygulanamadı anlamına gelir. Bu hatanın en olası nedeni, güvenlik duvarı yapılandırması ile ilgili bir sorun var. Sorunu gidermek için bu ayarları denetleyin:
  
- Bilgileri [Office 365 URL'leri ve IP adres aralıkları](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) ile güvenlik duvarı yapılandırmanızı doğrulayın
    
- Hata Exchange çevrimiçi koruma (EOP) belirli ise, daha önce bir değişiklik [Exchange çevrimiçi koruma IP adresleri](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)için bildirildi.
    
- Internet servis sağlayıcınıza (ISS) bağlantı noktası engellemediğinden emin olun.
    
- Bağlayıcılar, akıllı ana bilgisayar ve hedef sunucu ayarlarını doğrulayın.
    
Not Bu yolla *gelen* bağlantıları Office 365 engellemez. 
  

