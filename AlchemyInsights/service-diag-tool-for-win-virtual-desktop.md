---
title: Sanal Masaüstü için Windows tanılama aracı
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052406"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Sanal Masaüstü için Windows tanılama aracı

Windows Sanal Masaüstü (WVD), yöneticilerin tek bir arabirim üzerinden hataları tanımlamalarına olanak sağlayan bir tanılama aracı sunar. Bu araç, biri tarafından WVD rolü atandığı zaman tanılamayla ilgili bilgileri günlüğe kaydeder. Her günlükte etkinlikle ilgili WVD rolü, oturum sırasında görünen hata iletileri ve kiracı ve kullanıcıyla ilgili bilgiler yer alır. Azure Log Analytics, tanılama aracı tarafından oluşturulan etkinlik günlüğünü yakalamak için ya da kullanılabilir. Bunu şu şekilde yapabilirsiniz:

1. Azure portalı veya depolama alanı ile [bir Log](https://go.microsoft.com/fwlink/?linkid=2129500) Analytics [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Bağlan Windows Azure Monitor'a kullanın.](https://go.microsoft.com/fwlink/?linkid=2129913) Çalışma alanı kimliği ve Birincil Anahtar'a sahip olmak. Kurulum sihirbazı aracıyı doğru biçimde yapılandırmak ve Azure Monitor'la iletişim kura olduğundan emin olmak için bu bilgiye gerekmektedir.
1. [Tanılama verilerini çalışma alanınıza bastırın.](https://go.microsoft.com/fwlink/?linkid=2128284) Tanılama verilerini WVD kiracıdan çalışma alanınız için Log Analytics'e İtebilirsiniz.
1. WVD [ile ilişkili](https://go.microsoft.com/fwlink/?linkid=2128338) olarak iç veya dış olan sorunları tanıyın ve tanıyın.

WVD'de hizmet tanılama aracını yapılandırma hakkında daha fazla bilgi edinmek için [bkz. Tanılama özelliği için Log Analytics'i kullanma.](https://go.microsoft.com/fwlink/?linkid=2128084)
