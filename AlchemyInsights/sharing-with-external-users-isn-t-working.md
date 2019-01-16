---
title: Dış kullanıcılarla paylaşma çalışmıyor
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28318140"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>SharePoint içerik dış kullanıcılarla paylaşma sorunlarını düzeltme

Dış paylaşımı, kuruluşunuz için açık olduğundan emin olun:
  
1. Git [Hizmetleri &amp; Eklentileri Office 365 Yönetim Merkezi sayfasında](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ve **Siteler**düğmesini tıklatın.
    
2. "Aç." ayarı açık olduğundan emin olun "Varolan yalnızca dış kullanıcılar" seçilirse, dış kullanıcının Office 365 Yönetim Merkezi'nde listelenen olduğundan emin olun.
    
Site için dış paylaşımı açık olduğundan emin olun. Klasik site koleksiyonu için:
  
1. Sol bölmede, Klasik SharePoint Yönetim Merkezi **site koleksiyonları**' ı tıklatın.
    
2. Siteyi veya siteleri seçin ve Şerit üzerinde **Paylaşım**' ı tıklatın.
    
Bir Office 365 grubuna ait bir ekip sitesi veya bir iletişim sitesi için:
  
- Kuruluş çapında ayar oturum gerektirmeyen bağlantılar kullanarak dosya paylaşımı izin vermediği sürece bu yeni site türleri aynı paylaşım kuruluş çapında ayarınız olarak ayarına sahiptir. Bu durumda, siteler oturum yeni ve varolan dış kullanıcılar ile paylaşılmasına izin verecek. Belirli sitelerin ayarını değiştirmek için yeni SharePoint Yönetim Merkezi (Önizleme) veya PowerShell kullanın. [Daha fazla bilgi edinin](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Dış paylaşım ayarı herhangi bir site için kuruluş çapında ayarından daha fazla olmayacak izin veren ancak kuruluş çapında ayarınızı daha kısıtlayıcı olabilir. 
  

