---
title: Windows 10 cihazlarını yapılandırmak için Microsoft Intune güvenlik taban çizgilerini kullanma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696385"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Windows 10 cihazlarını yapılandırmak için Microsoft Intune güvenlik taban çizgilerini kullanma

Intune güvenlik taban çizgisi, kullanıcıların ve cihazların korunmasına yardımcı olur. Güvenlik taban çizgisi, Windows ayarlarının bilinen bir ayar grubunu ve ilgili güvenlik ekipleri tarafından önerilen varsayılan değerleri uygulamak için kullanılan önceden yapılandırılmış gruplarıdır. Intune'da bir güvenlik temeli profili oluşturarak, birden çok cihaz yapılandırma profili içeren bir şablon oluşturabilirsiniz.

Güvenlik taban çizgilerini kullanıcı veya cihaz gruplarına dağıtsanız, ayarlar Windows 10 veya daha sonraki sürümlerde çalıştıran cihazlara uygulanır. Örneğin, Microsoft mobil cihaz yönetimi (MDM) güvenlik temeli (1) çıkarılabilir sürücüler için BitLocker'ı otomatik olarak etkinleştirir, (2) cihazın kilidini açmak için parolayı gerektirir ve (3) temel kimlik doğrulamasını devre dışı bırakır. Ortamınız için varsayılan bir değer işe yaramadı mı, ihtiyacınız olan ayarları uygulamak için taban çizgisini özelleştirebilirsiniz.

Güvenlik taban çizgisi, Microsoft 365'te uç- uç güvenli iş akışı kurulmasına da yardımcı olur. Bu işlevin bazı avantajları aşağıda ve aşağıda ve ve aşağıda ve ve listelerde ve listelerde yer alan bilgiler ve bilgileri bulunmaktadır:
- Güvenlik temeli, güvenliği etkileyen ayarlarla ilgili en iyi yöntemleri ve önerileri içerir. Intune, grup ilkeleri için taban çizgisi oluşturan Windows güvenlik ekibiyle ortak çalışmalarından dolayı, bu öneriler sağlam bir kılavuza ve kapsamlı deneyime dayalıdır.
- Intune'da yeniyseniz ve nereden başlayacağınıza emin değilseniz, güvenlik taban çizgisi hızla güvenli bir profil oluşturmanıza ve dağıtmanıza yardımcı olur.
- Şu anda grup ilkesi kullanıyorsanız, intune'a yönetim amacıyla bu güvenlik taban çizgileriyle daha kolay bir şekilde devam etmektir, çünkü bu güvenlik taban değerleri Intune'da yerleşiktir ve yönetim için en son özellikleri içerir.

Daha fazla bilgi için Windows güvenlik [taban çizgilerine ve](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) Mobil cihaz [yönetimine bakın.](https://docs.microsoft.com/windows/client-management/mdm/)