---
title: 1065 EOP giden IP adresi aralıklarını kullanımdan çıkmaMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031282"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP giden IP adresi aralıklarını kullanımdan çıkma

Kuruluşta olası bir sorun algıladık. (26 Ekim 2018'e kadar düzeltilemedik), şirket içi veya dış hedeflerinize posta akışınızı bozabilirsiniz. Daha önce belirtildiği gibi, IP adresi aralığı yönetimini basitleştirmek için, ip adresi yönetiminin dışında e-posta göndermek ve almak için kullanılan Exchange Online Protection (EOP) IP adresi aralıklarını Microsoft 365. Çözümlememiz, posta akış bağlayıcılarında yapılandırmış olduğunuz dış e-posta kaynaklarından veya hedeflerinden birinin burada gösterilen [](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)IP adresi aralıklarından bağlantıları kabul etmemektedir.

Bu kaynak ve hedeflerin yayımlanmış tüm EOP IP adreslerine ve bu adreslere bağlantı kabul edeceklerinden emin olmak için 26 [Ekim'den önce harekete geçebilirsiniz.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Bu değişiklik hakkında daha fazla bilgi için lütfen bkz. İleti Merkezi [gönderileri MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)veya [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Not:** Uç nokta güncelleştirmeleri için daha önce HTML, XML ve RSS aracılığıyla IP veya URL yayımlama kullandıysanız, bu tür güncelleştirmeleri otomatik yapmak için de yeni web hizmetlerine geçişlisiniz. Daha fazla bilgi için [bkz. Microsoft 365 uç nokta kategorilerini Microsoft 365 IP Adresi ve URL web hizmetinin adı.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
