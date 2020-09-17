---
title: 1065 EOP giden IP adresi rangesMC146155
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
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806815"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Giden IP adresi aralıklarının kullanımdan kaldırılması

Kuruluşunuzda (Ekim 26 ' ya kadar düzeltilmez, 2018) Şirket içi veya dış hedeflerine posta akışını bozabilecek olası bir sorun algıladık. Daha önce, IP adres aralığı yönetimini basitleştirmek amacıyla, Microsoft 365 dışında e-posta göndermek ve almak için kullanılan Exchange Online Protection (EOP) IP adresi aralıklarını birleştiriyoruz. Çözümümüz, posta akışı bağlayıcılarının, [burada](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)gösterilen IP adresi aralıklarından gelen bağlantıları kabul etmediği anlamına gelir.

Bu kaynakların ve hedeflerin tüm [yayımlanan EOP IP adreslerine](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)yönelik bağlantıları kabul edeceği Için, Ekim 26 ' dan önce hareket edin.

Bu değişiklik hakkında daha fazla bilgi için bkz: Message Center gönderileri [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)veya [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Not**: daha önce HTML, XML ve RSS aracılığıyla uç nokta güncelleştirmelerinde IP veya URL yayımlamayı kullandıysanız, bu tür güncellemeleri otomatikleştirmek için yeni Web hizmetlerine de geçiş yapmalısınız. Daha fazla bilgi için bkz: [microsoft 365 uç nokta kategorileri ve microsoft 365 IP adresi ve URL Web hizmeti](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
