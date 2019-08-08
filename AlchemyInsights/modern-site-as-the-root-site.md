---
title: Modern site kök site olarak
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232735"
---
# <a name="modern-site-as-root-site"></a>Modern site kök site olarak

Biz ürün için Klasik site kök sitenizin modern bir site ile takas etmek izin veren yeni bir özellik başlamıştır. [Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) konumunu başka bir siteye sahip bir site, özgün site Arşivlerken takas etmek için kullanın. Ekip sitesi (bir gruba bağlı değil) hem de iletişim Site için kullanılabilir. 

>[!Important]
> Modern bir iletişim sitesi oluşturmak için Klasik kök site silmeyin. Bu Microsoft tarafından desteklenmez. Siteyi geri yüklemek veya aynı URL'de yeni bir site oluşturmak kadar kök site silindiğinde tüm SharePoint siteleri, kuruluşunuzdaki tüm kullanıcılar için erişilebilir hale getirir. Biz bu özellik ileti merkezi aracılığıyla iletişim. Özelliği, Kiracı kısa bir süre sonra açık olması için beklemeniz gerekir.

## <a name="known-issues-with-swapping-sites"></a>Takas siteleri ile ilgili bilinen sorunlar
- Hedef site kısa bir süre için bir "not found" (HTTP 404) hata döndürebilir.
- İçerik arama dizini güncelleştirmek için recrawled gerekecek. Burada gereken el ile hiçbir adım, bu otomatik olarak yapılacaktır.
- "Statik" bağlantıları (örneğin, dosya eşitleme ve OneNote dosyaları) bağımlı bir şey elle düzeltilmesi gerekir.
- Project Server siteleri doğru hala ilişkili olduklarından emin olmak için doğrulanması gerekebilir. 
