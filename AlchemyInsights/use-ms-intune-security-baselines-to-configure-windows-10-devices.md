---
title: Cihazları Microsoft Intune için güvenlik taban çizgilerini Windows 10 kullanma
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
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104364"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Cihazları Microsoft Intune için güvenlik taban çizgilerini Windows 10 kullanma

Intune güvenlik taban çizgisi, kullanıcıları ve cihazları korumaya yardımcı olur. Güvenlik taban Windows, bilinen bir grup ayarın ve ilgili güvenlik ekipleri tarafından önerilen varsayılan değerlerin kullanılması için kullanılan, ayarların önceden yapılandırılmış gruplarıdır. Intune'da güvenlik taban çizgisi profili oluşturarak, birden çok cihaz yapılandırma profili içeren bir şablon oluşturabilirsiniz.

Kullanıcı veya cihaz gruplarına güvenlik taban çizgilerini dağıtıyorken, ayarlar daha sonra veya birden çok Windows 10 uygulanır. Örneğin, MDM Güvenlik Temeli (1) çıkarılabilir sürücüler için BitLocker'ı otomatik olarak etkinleştirir, (2) cihazın kilidini açmak için parolayı gerektirir ve (3) temel kimlik doğrulamayı devre dışı bırakır. Ortamınıza bir varsayılan değer çalışmazsa, ihtiyacınız olan ayarları uygulamak için temeli özelleştirin.

Güvenlik taban çizgisi, aynı zamanda iş akışlarında uç- uç güvenli iş akışı Microsoft 365. Aşağıdaki avantajlardan bazılarıdır:

- Güvenlik temeli, güvenliği etkileyen en iyi yöntemleri ve ayarların önerilerini içerir. Intune, grup ilkeleri için taban Windows oluşturan güvenlik ekibiyle ortak olduğundan, bu öneriler sağlam kılavuza ve kapsamlı deneyime dayalıdır.
- Intune'da yeniyseniz ve nereden başlayacağınıza emin değilseniz, güvenlik taban çizgisi hızla güvenli bir profil oluşturmanıza ve dağıtmanıza yardımcı olur.
- Şu anda bir grup ilkesi kullanıyorsanız, güvenlik taban çizgileriyle Intune'da yerleşik olarak olduğundan ve yönetim için en yeni özellikleri içermelerine neden olduğundan, yönetim amacıyla Intune'a varma işlemi çok daha kolaydır.

Daha fazla bilgi edinmek için [bkz. Windows temelleri ve](https://go.microsoft.com/fwlink/?linkid=2141503) [Mobil cihaz yönetimi.](https://go.microsoft.com/fwlink/?linkid=2141701)