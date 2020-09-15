---
title: Dış kullanıcılarla paylaşım çalışmıyor
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691595"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Dış kullanıcılarla SharePoint içeriğini paylaşma sorunlarını giderme

Kuruluşunuzda dış paylaşımın açık olduğundan emin olun:
  
1. [ &amp; Microsoft 365 Yönetim Merkezi 'nde hizmetler eklentileri sayfasına](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)gidin ve **siteler**'e tıklayın.
    
2. Ayarın "açık" olduğundan emin olun. "Yalnızca mevcut dış kullanıcılar" seçiliyse, dış kullanıcının Microsoft 365 Yönetim merkezinde listelendiğinden emin olun.
    
Site için dış paylaşımın açık olduğundan emin olun. Klasik site koleksiyonu için:
  
1. Yeni SharePoint Yönetim merkezinde, sol bölmede **siteler**'e tıklayın.
    
2. Siteyi veya siteleri seçin ve şeritte **Paylaşım**'a tıklayın.
    
Microsoft 365 grubuna veya iletişim sitesine ait bir ekip sitesi için:
  
- Kuruluş genelindeki ayarlar, oturum açma gerektirmeyen bağlantılar kullanarak dosya paylaşmaya izin vermediği sürece, bu yeni site türlerinin kuruluş genelindeki ayarı ile aynı paylaşım ayarı vardır. Bu durumda, siteler yeni ve oturum açan dış kullanıcılarla paylaşmaya izin verir. Belirli sitelerin ayarını değiştirmek için yeni SharePoint Yönetim merkezini veya PowerShell 'i kullanın. [Daha fazla bilgi edinin](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Herhangi bir site için dış paylaşım ayarı, kuruluş genelindeki ayardan daha kısıtlayıcı olabilir, ancak kuruluş genelindeki ayardan daha fazla izin vermez. 
  

