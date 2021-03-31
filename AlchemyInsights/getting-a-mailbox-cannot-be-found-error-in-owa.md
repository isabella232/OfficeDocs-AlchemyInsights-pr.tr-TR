---
title: 126 OWA'da Posta Kutusu alma hatası bulunamıyor mu?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426682"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Web üzerinde Outlook'ta posta kutusu bulunamadı hatası mı alasınız?

Web üzerinde Outlook kullanıyorsanız ve hata için bir Posta Kutusu bulunamadı varsa, Web üzerinde **Outlook'a** bağlanmak için kullanılan hesabın Exchange Online lisansı yoktur ve dolayısıyla hesapla ilişkilendirilmiş posta kutusu yoktur. Yöneticiniz aşağıdaki adımları kullanarak hesabınıza lisans atayabilirsiniz:

1. Microsoft [365 yönetim](https://portal.office.com/adminportal/home#/homepage) merkezini açın  ve Kullanıcılar  bölümünün altında Etkin kullanıcılar'a gidin ve hatayı gören kullanıcıyı seçin.

2. Açılan kullanıcı sayfasında Lisanslar ve  Uygulamalar bölümüne gidin, uygun  Konum değerini seçin ve Exchange Online içeren bir lisans attayın (ayrıntılarını görmek için lisansı genişletin). Bitirdikten sonra, Değişiklikleri **kaydet'e tıklayın.**

Bazı durumlarda, lisans bir kullanıcı hesabına zaten atanmışsa, lisansın kaldırılması ve yeniden atanmış olması sorunu çözmenize ve sistemde düzgün bir şekilde sağlanmasına yardımcı olur: 

- M365 Exchange Online (ve varsa diğer) aboneliklerinizi güncel olup olmadığını ve henüz süresinin dolmadı olup olmadığını kontrol edin.

Aboneliğinizin süresinin dolmamış olduğundan ve kullanıcı hesabına geçerli bir lisans atanmalarından emin olduktan sonra, lisansın sağlanması 24 saate kadar sürebilir, bu nedenle sorununuzu çözmeyi beklemeniz gerekir. Daha fazla bilgi için bkz. [Lisans atama ve yönetme.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)