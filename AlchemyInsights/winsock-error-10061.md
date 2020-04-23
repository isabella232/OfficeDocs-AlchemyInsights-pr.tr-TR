---
title: 1554 Winsock hatası 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766189"
---
# <a name="winsock-error-10061"></a>Winsock hatası 10061

Bu hata kodu, Microsoft'un hedef ana bilgisayarla bir TCP soketi (bağlantı) kuramadığı anlamına gelir. Bu hatanın en olası nedeni güvenlik duvarı yapılandırmanızla ilgili bir sorundur. Sorunu gidermek için şu ayarları denetleyin:

- Güvenlik duvarı yapılandırmanızı Microsoft [365 URL'leri ve IP adres aralıklarında](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) bulunan bilgilerle doğrulayın

- Hata Exchange Online Protection 'a (EOP) özgüyse, daha önce Exchange [Online Protection IP adreslerinde](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)bir değişiklik için bilgilendirilmeniz gerekirdi.

- Internet Servis Sağlayıcınızın (ISS) bağlantı noktasını engellemediğini doğrulayın.

- Bağlayıcılarınızdaki akıllı ana bilgisayar ve hedef sunucu ayarlarını doğrulayın.

Microsoft 365'in *gelen* bağlantıları bu şekilde engellemediğini unutmayın.
