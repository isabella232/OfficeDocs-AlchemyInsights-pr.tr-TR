---
title: Kök site olarak modern site
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753924"
---
# <a name="modern-site-as-root-site"></a>Kök site olarak modern site

Biz modern bir site ile klasik site [kök sitesi takas](https://docs.microsoft.com/sharepoint/modern-root-site)sağlayacak yeni bir özellik piyasaya başladı. Orijinal siteyi arşivlerken bir sitenin konumunu başka bir siteyle değiştirmek için [Invoke-SPOSiteSwap'ı](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) kullanın. Hem Takım Sitesi (bir gruba bağlı değil) hem de İletişim Sitesi için kullanılabilir.

>[!Important]
> Modern bir İletişim Sitesi oluşturmak için klasik kök sitenizi silmeyin. Bu Microsoft tarafından desteklenmez. Siteyi geri yükleyene veya aynı URL'de yeni bir site oluşturana kadar, kök siteyi sevebilmek, kuruluşunuzdaki tüm SharePoint sitelerini tüm kullanıcılar tarafından erişilemez hale getirir. Bu özelliği mesaj merkezi aracılığıyla ileteceğiz. Özelliğin kısa süre içinde kiracınızda açık olmasını beklemelisiniz.

## <a name="known-issues-with-swapping-sites"></a>Siteleri değiştirme yle ilgili bilinen sorunlar
- Hedef site kısa bir süre için bir "bulunamadı" (HTTP 404) hatası döndürebilir.
- Arama dizinini güncelleştirmek için içeriğin yeniden taranması gerekir. Burada herhangi bir manuel adım gereklidir, bu otomatik olarak yapılacaktır.
- "Statik" bağlantılara (Dosya Eşitlemi ve OneNote dosyaları gibi) bağlı olan her şeyin el ile düzeltilmesi gerekir.
- Project Server sitelerinin hala doğru ilişkili olduğundan emin olmak için doğrulanması gerekebilir. 
