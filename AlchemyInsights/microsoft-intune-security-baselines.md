---
title: Cihazları Microsoft Intune için güvenlik taban çizgilerini Windows 10 kullanma
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 0a89b121f2f425b0a81fa250650f108e9af48c9da39dfc8a62b07541d3a6c3dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098082"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Cihazları Microsoft Intune için güvenlik taban çizgilerini Windows 10 kullanma

Intune güvenlik taban çizgisi, kullanıcıları ve cihazları korumaya yardımcı olur. Güvenlik taban Windows, bilinen bir grup ayarı ve ilgili güvenlik ekipleri tarafından önerilen varsayılan değerleri uygulamak için kullanılan önceden yapılandırılmış ayarlardır. Intune'da güvenlik taban çizgisi profili oluşturarak, birden çok cihaz yapılandırma profili içeren bir şablon oluşturabilirsiniz.

Kullanıcı veya cihaz gruplarına güvenlik taban çizgilerini dağıtıyorken, ayarlar daha sonra veya birden çok Windows 10 uygulanır. Örneğin, Microsoft mobil cihaz yönetimi (MDM) güvenlik temeli çıkarılabilir sürücüler için BitLocker'ı otomatik olarak etkinleştirir, cihazın kilidini açmak için parolayı gerektirir ve temel kimlik doğrulamayı devre dışı bırakır. Ortamınız için varsayılan değer işe yaramadı mı, ihtiyacınız olan ayarları uygulamak için temeli özelleştirebilirsiniz.

Güvenlik taban çizgisi, aynı zamanda iş akışlarında uç- uç güvenli iş akışı Microsoft 365. Güvenlik temeli, güvenliği etkileyen en iyi yöntemleri ve ayarların önerilerini içerir. Intune, grup ilkeleri Windows temeller oluşturan güvenlik ekibiyle ortak çalışmalarına sahip olur; bu nedenle bu öneriler sağlam kılavuzdan ve kapsamlı deneyimden temel almaktadır.

Intune'da yeniyseniz ve nereden başlayacağınıza emin değilseniz, güvenlik taban çizgisi hızla güvenli bir profil oluşturmanıza ve dağıtmanıza yardımcı olur. Şu anda bir grup ilkesi kullanıyorsanız, intune'da yerleşik olarak bulunan ve en yeni yönetim özelliklerini içeren bu ilkeler, güvenlik taban çizgileriyle yönetim amacıyla Intune'a olmak çok daha kolaydır.

Daha fazla bilgi edinmek için [bkz. Windows temelleri ve](/windows/security/threat-protection/windows-security-baselines) [Mobil cihaz yönetimi.](/windows/client-management/mdm/)

