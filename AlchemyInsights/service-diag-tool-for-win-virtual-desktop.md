---
title: Windows sanal masaüstü için hizmet Tanılama Aracı
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680235"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Windows sanal masaüstü için hizmet Tanılama Aracı

Windows sanal masaüstü (WVD), yöneticilerin hataları tek bir arabirim aracılığıyla belirlemesine olanak tanıyan bir tanılama aracı sunar. Bu araç, WVD rolüne atanan bir kullanıcı tarafından WVD kullanıldığında tanılamaların ilgili bilgilerini günlüğe kaydeder. Her günlükte, faaliyette yer alan WVD rolüyle ilgili bilgiler, oturum sırasında görünen hata mesajları ve kiracı ile Kullanıcı hakkındaki bilgiler yer alır. Azure Log Analytics, tanılama aracı tarafından oluşturulan etkinlik günlüğünü yakalamak üzere yapılandırılabilir. Bunu şu şekilde yapabilirsiniz:

1. [Azure portalı](https://go.microsoft.com/fwlink/?linkid=2129500) veya [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)ile bir Log Analytics çalışma alanı oluşturun.
1. [Windows bilgisayarlarını Azure monitöre bağlama](https://go.microsoft.com/fwlink/?linkid=2129913). Çalışma alanınızın KIMLIĞINI ve çalışma alanınızın birincil anahtarını edinin. Kurulum Sihirbazı, aracıyı düzgün bir şekilde yapılandırmak ve Azure Monitor ile iletişim kurabildiğinden emin olmak için bu bilgiye ihtiyaç duyar.
1. [Tanılama verilerini çalışma alanınıza gönderin](https://go.microsoft.com/fwlink/?linkid=2128284). WVD kiracınızdaki tanılama verilerini çalışma alanınızın günlük çözümlemelerini gönderebilirsiniz.
1. WVD ile ilgili iç veya dış [sorunları tanımlayın ve tanılayın](https://go.microsoft.com/fwlink/?linkid=2128338) .

WVD için hizmet Tanılama Aracı 'nı yapılandırma hakkında daha fazla bilgi edinmek için, [Tanılama özelliği Için Günlük Analizi kullanma](https://go.microsoft.com/fwlink/?linkid=2128084)konusuna bakın.
