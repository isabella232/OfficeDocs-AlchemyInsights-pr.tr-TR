---
title: Harici kullanıcılarla paylaşmak çalışmıyor
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582795"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>SharePoint içeriğini dış kullanıcılarla paylaşan sorunları giderme

Kuruluşunuz için dış paylaşımın açık olduğundan emin olun:
  
1. [ &amp; Microsoft 365 yönetici merkezindeki Hizmetler eklentileri sayfasına](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)gidin ve **Siteler'i**tıklatın.
    
2. Ayarın "Açık" olarak döndürüldiğinden emin olun. "Yalnızca varolan harici kullanıcılar" seçilirse, dış kullanıcının Microsoft 365 yönetici merkezinde listelenmiş olduğundan emin olun.
    
Site için dış paylaşımın açık olduğundan emin olun. Klasik bir site koleksiyonu için:
  
1. Yeni SharePoint yönetici merkezinde, sol **bölmede, siteleri**tıklatın.
    
2. Siteyi veya siteleri seçin ve şeritte **Paylaşım'ı**tıklatın.
    
Microsoft 365 grubuna veya bir iletişim sitesine ait bir ekip sitesi için:
  
- Kuruluş genelinde ayar oturum açma gerektirmeyen bağlantıları kullanarak dosyaların paylaşılmasına izin vermese, bu yeni site türleri kuruluş genelindeki ayarınızla aynı paylaşım ayarına sahiptir. Bu durumda, siteler oturum kuran yeni ve varolan harici kullanıcılarla paylaşıma izin verir. Belirli sitelerin ayarını değiştirmek için yeni SharePoint yönetici merkezini veya PowerShell'i kullanın. [Daha fazla bilgi edinin](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Herhangi bir sitenin dış paylaşım ayarı kuruluş çapındaki ayarınızdan daha kısıtlayıcı olabilir, ancak kuruluş genelindeki ayarından daha izin verilebilir. 
  

