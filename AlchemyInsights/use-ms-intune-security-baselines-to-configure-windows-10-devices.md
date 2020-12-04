---
title: Windows 10 cihazlarını yapılandırmak için Microsoft Intune güvenlik temellerini kullanma
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573785"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Windows 10 cihazlarını yapılandırmak için Microsoft Intune güvenlik temellerini kullanma

Intune güvenlik temelleri, kullanıcıları ve cihazları korur. Güvenlik temelleri, bilinen bir ayar grubunu uygulamak için kullanılan önceden yapılandırılmış gruplar ve ilgili güvenlik ekipleri tarafından önerilen varsayılan değerleri, Windows ayarları 'nı uygulamak için kullanılır. Intune 'da bir güvenlik temel profili oluşturarak, birden çok cihaz yapılandırma profilinden oluşan bir şablon oluşturacaksınız.

Güvenlik temellerini Kullanıcı veya cihaz gruplarına dağıtırken, ayarlar Windows 10 veya üstünde çalışan cihazlara uygulanır. Örneğin, MDM güvenlik temeli otomatik olarak (1) çıkarılabilir sürücüler için BitLocker 'ı, (2) cihazın kilidini açmak için parola gerektirir ve (3) temel kimlik doğrulamasını devre dışı bırakır. Varsayılan bir değer ortamınızda çalışmazsa, ihtiyacınız olan ayarları uygulamak için taban çizgisini özelleştirin.

Güvenlik temelleri, Microsoft 365 'da uçtan uca güvenli bir iş akışı oluşturmaya da yardımcı olur. Aşağıda, bunun avantajları verilmiştir:

- Güvenlik temeli, güvenliği etkileyen ayarlar için en iyi yöntemleri ve önerileri içerir. Intune, Grup ilkeleri için taban çizgileri oluşturan Windows Güvenlik ekibinden gelen iş ortakları nedeniyle, bu öneriler düz kılavuza ve kapsamlı deneyimlere dayanır.
- Intune 'a yeni bağlıysanız ve nereden başlayacağınızı bilmiyorsanız, güvenlik temelleri hızlı bir şekilde güvenli bir profil oluşturup dağıtmanızı sağlayacaktır.
- Şu anda bir grup ilkesi kullanıyorsanız, yönetim amaçları için Intune 'a geçirmek, güvenlik temelleriyle çok daha kolaydır çünkü bu, Intune 'da yerleşik olmaları ve yönetim için uçtan uca özellikler içermektedir.

Daha fazla bilgi edinmek için [Windows güvenlik temelleri](https://go.microsoft.com/fwlink/?linkid=2141503) ve [mobil cihaz yönetimi](https://go.microsoft.com/fwlink/?linkid=2141701)'ne bakın.