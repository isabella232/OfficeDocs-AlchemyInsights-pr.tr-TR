---
title: Geçici Microsoft 365 sorunlarını giderme Ne üzgünüz, geçici sunucu sorunları iletisiyle karşıda
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744687"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Aşağıdaki Microsoft 365 "Üzgünüz, geçici sunucu sorunlarımız var" iletisi

Not: Windows'ın eski bir sürümünü (örneğin, Windows 7 SP1, Windows Server 2008 R2) kullanıyorsanız, kolay düzeltmeyi kullanarak TLS 1.2'yi varsayılan olarak etkinleştirin. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Daha fazla bilgi için bkz. Windows'da WinHTTP'da varsayılan güvenli protokol olarak [TLS 1.1 ve TLS 1.2'yi](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)etkinleştirmek için Windows.

Bu iletiyi alırsanız, şunları deneyin:

1. Güvenlik duvarınızı, virüsten koruma yazılımınızı ve proxy ayarlarınızı kontrol edin ve bu uygulamaların İnternet erişimini engelleme Microsoft 365 yapın. Bkz. [URL'ler ve IP adresi aralıkları.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Başlangıç **Çalıştırma'ya**  >  **gidin** ve **services.msc yazın.** Aşağıdaki hizmetlerin hepsinin çalıştırlı olduğundan emin olun:
    - Ağ Bağlantılı Cihazlar Otomatik Kurulumu
    - Ağ Listesi Hizmeti
    - Ağ Konumu Farkındalığı
    - Windows Olay Günlüğü

Bu hizmetlerden biri çalışmıyorsa, başlatmayı deneyin. Hizmeti başlatmayla ilgili bir sorun varsa yükseltilmiş izinlerle bir komut istemi açarak aşağıdaki komutu çalıştırın:

**sfc /scannow**

Bu komut tamamdikten sonra bilgisayarı yeniden başlatın.

Ayrıntılı bilgi için [bkz. "Ne üzgünüz, hesabınıza bağlana üzgünüz. 'i etkinleştirirken lütfen daha sonra yeniden deneyin" hatası.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)