---
title: Performans sorunları-SharePoint veya OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911862"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint kullanıcı OneDrive, erişilemez veya kullanılamaz durumda olabilir

SharePoint veya OneDrive, erişilemez veya kullanılamaz olabilir ya da çeşitli nedenlerle hizmet kullanılamayabilir veya 503 hata bunlardan oluşabilir:
  
- SharePoint veya OneDrive siteniz birden çok kullanıcı için yavaş veya geciktirilirse, kullanıcıların sitelere veya site içeriğine erişirken aralıklı olarak gecikmeler veya gezinti hataları ile SharePoint bir geçici hizmet sorunu OneDrive olabilir. Hizmet durumu [panosuna bakarak,](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) kuruma etki veriniz olup yardımcı olduğunu kontrol edin.
  
- Kullanıcılar, başka bir siteyi ziyaret etmek veya sitelere gitmek isterken *503* SharePoint meşgul OneDrive alabilirsiniz. Bu hataya, çalışma hizmeti içindeki azaltma neden SharePoint olabilir. SharePoint Online, SharePoint Online hizmetinin en iyi düzeyde performans ve güvenilirliğini sürdürmesi için kısıtlama kullanıyor. Kısıtlama işlemi, kaynakların aşırı kullanımını önlemek için kullanıcı eylemi veya eşzamanlı çağrı (betik veya kod ile) sayısını sınırlar. Azaltma hakkında daha fazla bilgi için bkz. [SharePoint Online'da azaltmaya veya engellemeye SharePoint.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Klasik veya **modern** bir site veya **sayfada** yavaş SharePoint, sayfaları [çözümlemek](https://aka.ms/perftool) için Sayfa Tanılama aracını kullanın.
  
- Genel yavaş performansla hâlâ devam ediyorsanız, lütfen bu makalenin sonundaki kaynakları gözden geçirme: SharePoint Online için [performans ayarlamaya giriş](https://go.microsoft.com/fwlink/?linkid=2024334)
  