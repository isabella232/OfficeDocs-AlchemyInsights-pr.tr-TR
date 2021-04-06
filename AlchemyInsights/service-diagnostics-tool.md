---
title: Windows Sanal Masaüstü için hizmet tanılama aracı
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596044"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Windows Sanal Masaüstü için hizmet tanılama aracı

Windows Sanal Masaüstü (WVD), yöneticilerin hataları tek bir arabirim üzerinden tanımlamalarına olanak sağlayan bir tanılama aracı sunar. Bu araç, WVD rolü atanan biri tarafından her WVD kullanılasında tanılamayla ilgili bilgileri günlüğe kaydeder. Her günlük, etkinlikte yer alan WVD rolü, oturum sırasında görünen hata iletileri ve kiracı ve kullanıcı hakkında bilgi içerir. Azure Log Analytics, aşağıdaki adımlarla tanılama aracı tarafından oluşturulan etkinlik günlüğünü yakalamak üzere yalndırabilirsiniz:

1. [Azure portalı](https://go.microsoft.com/fwlink/?linkid=2129500) veya Azure PowerShell ile bir Log Analytics çalışma alanı [oluşturun.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Windows bilgisayarlarını Azure Monitor'e bağlama.](https://go.microsoft.com/fwlink/?linkid=2129913) Çalışma alanı kimliğini ve çalışma alanı birincil anahtarını alırsınız. Kurulum sihirbazı aracıyı düzgün bir şekilde yapılandırmak ve Azure Monitor ile iletişim kuraya sahip olduğundan emin olmak için bu bilgiye gerekmektedir.

1. [Tanılama verilerini çalışma alanınıza bastırın.](https://go.microsoft.com/fwlink/?linkid=2128284) Tanılama verilerini WVD kiracıdan çalışma alanınız için Log Analytics'e İtebilirsiniz.

1. WVD [ile](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) ilişkili olarak iç veya dış sorunları tanılar ve tanılar.

WVD için hizmet tanılama aracını yapılandırma hakkında daha fazla bilgi edinmek için bkz. Tanılama özelliği için Log Analytics'i kullanma.