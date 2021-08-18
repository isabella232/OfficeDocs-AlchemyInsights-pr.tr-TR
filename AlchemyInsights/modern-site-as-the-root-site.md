---
title: Kök site olarak modern site
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327622"
---
# <a name="modern-site-as-root-site"></a>Kök site olarak modern site

Klasik site kök sitenizi modern bir siteyle değiştirmenizi sağlayacak [yeni bir özelliğin yeni bir özelliğinin ne olduğu hakkında bilgi edinmaya başladık.](https://docs.microsoft.com/sharepoint/modern-root-site) Özgün siteyi arşivlerken bir sitenin konumunu başka bir siteyle değiştirmek için [Invoke-SPOSiteSwap'ı](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) kullanın. Hem Ekip Sitesi (bir gruba bağlı değil) hem de İletişim Sitesi için kullanılabilir.

**Önemli:** Modern bir İletişim Sitesi oluşturmak için klasik kök sitesini silmeyin. Bu Microsoft tarafından desteklenmiyor. Kök sitenin silinmesi, SharePoint siteyi geri yükleyene veya aynı URL'de yeni bir site oluşturana kadar, tüm kullanıcılar tarafından erişilemez hale gelecektir. Bu özelliği ileti merkezi aracılığıyla iletiriz. Özelliğin kiracınıza kısa süre içinde açık olmasını bekleyebilirsiniz.

## <a name="known-issues-with-swapping-sites"></a>Site değiştirmeyle ilgili bilinen sorunlar
- Hedef site kısa bir süre için "bulunamadı" (HTTP 404) hatası döndürür.
- Arama dizinini güncelleştirmek için içeriğin yeniden akmış olması gerekir. Burada el ile herhangi bir adım gerekli değildir, bu işlem otomatik olarak yapılır.
- "Statik" bağlantılara (Dosya Eşitleme ve OneNote gibi) bağımlı olan her şeyin el ile düzeltilmesi gerekir.
- Project Hala doğru ilişkilendirillerinden emin olmak için sunucu sitelerinin doğrulanması gerekiyor olabilir. 
