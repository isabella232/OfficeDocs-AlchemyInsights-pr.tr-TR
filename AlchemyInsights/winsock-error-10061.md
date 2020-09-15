---
title: 1554 Winsock hata 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698882"
---
# <a name="winsock-error-10061"></a>Winsock hatası 10061

Bu hata kodu, Microsoft 'un hedef ana bilgisayarla TCP yuvası (bağlantı) kurmadığı anlamına gelir. Bu hatanın en olası nedeni, güvenlik duvarı yapılandırmanızla ilgili bir sorundur. Sorunu çözmek için şu ayarları işaretleyin:

- Güvenlik duvarı yapılandırmanızı [Microsoft 365 URL 'lerinde ve IP adresi aralıklarıyla](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) doğrulama

- Hata, Exchange Online Protection (EOP) için gerekliyse, daha önce [Exchange Online PROTECTION IP adreslerinde](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)bir değişiklik yapmanız istenir.

- Internet servis sağlayıcınızın (ISP) bağlantı noktasını engellemediğini doğrulayın.

- Bağlayıcılarınızın akıllı ana bilgisayar ve hedef sunucu ayarlarını doğrulayın.

Microsoft 365, *gelen* bağlantıları bu şekilde engellemez.
