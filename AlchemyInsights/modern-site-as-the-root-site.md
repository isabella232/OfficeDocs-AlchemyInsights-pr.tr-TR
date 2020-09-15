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
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666890"
---
# <a name="modern-site-as-root-site"></a>Kök site olarak modern site

[Klasik site kök sitenizi modern bir siteyle takas](https://docs.microsoft.com/sharepoint/modern-root-site)etme olanağı tanıyan yeni bir özellik piyasaya çıkarılacak. Özgün siteyi arşivlerken, bir sitenin konumunu başka bir siteyle değiştirmek için [çağır-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) 'ı kullanın. Hem ekip sitesi (gruba bağlı değil) hem de Iletişim sitesi için kullanılabilir.

>[!Important]
> Modern bir Iletişim sitesi oluşturmak için klasik kök sitenizi silmeyin. Bu, Microsoft tarafından desteklenmez. Kök site silindiğinde, siz siteyi geri yükleyinceye veya aynı URL 'de yeni bir site oluşturana kadar kuruluşunuzdaki tüm SharePoint sitelerinin tüm kullanıcılara erişilemez olmasını sağlayabilirsiniz. Bu özelliğe ileti merkezi aracılığıyla iletişim kuracağız. Bu özelliğin kiracınızda hemen açık olmasını beklemelisiniz.

## <a name="known-issues-with-swapping-sites"></a>Siteleri değiştirme ile ilgili bilinen sorunlar
- Hedef site kısa bir süre boyunca "bulunamadı" (HTTP 404) hatası döndürebilir.
- İçerik, arama dizinini güncelleştirmek için yeniden gezilecek. Burada el ile adım gerekmeyecektir, bu işlem otomatik olarak yapılır.
- "Statik" bağlantılara (dosya eşitleme ve OneNote dosyaları gibi) bağlı olarak, el ile düzeltilmesi gerekir.
- Project Server sitelerinin doğru ilişkilendirilmeleri için doğrulanması gerekebilir. 
