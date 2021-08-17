---
title: 1554 Winsock hatası 10061
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
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083250"
---
# <a name="winsock-error-10061"></a>Winsock hatası 10061

Bu hata kodu, Microsoft'un hedef ana bilgisayarla bir TCP yuva (bağlantı) kuramay olduğu anlamına gelir. Bu hatanın en olası nedeni, güvenlik duvarı yapılandırmanıza bağlı bir sorundur. Sorunu gidermek için şu ayarları kontrol edin:

- GÜVENLIK duvarı yapılandırmanızı URL'ler ve [IP Microsoft 365 bilgileriyle doğrulama](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Hata Exchange Online Protection (EOP) ile ilgili ise, daha önce IP adreslerinde bir değişiklik [size Exchange Online Protection gerekir.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- İnternet Servis Sağlayıcınızın (ISS) bağlantı noktasını engelleyeni olduğunu doğrulayın.

- Bağlayıcılar'daki akıllı ana bilgisayar ve hedef sunucu ayarlarını doğrulayın.

Bu Microsoft 365 gelen bağlantıları bu *şekilde* engellemez.
