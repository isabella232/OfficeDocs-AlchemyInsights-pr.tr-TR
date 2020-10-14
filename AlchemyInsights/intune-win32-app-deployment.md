---
title: Intune Win32 uygulama dağıtımı
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461996"
---
# <a name="intune-win32-app-deployment"></a>Intune Win32 uygulama dağıtımı

Microsoft Intune, MSI ve bunlarla sınırlı olmamak kaydıyla, Win32 uygulamalarına olanak tanır. Windows 10 cihazlarına dağıtılacak olan EXE. Kullanılan dağıtım mekanizması, hedef cihazda Intune yönetim uzantısının (IME) olmasını gerektirir. Bir Kullanıcı/cihaza PowerShell betiği veya Win32 uygulama dağıtımının hedeflenmesi sonucunda, IME otomatik olarak yüklenir.

Ayrıca, aşağıdakileri içeren Win32 uygulamalarını dağıtmak için karşılanması gereken bir dizi ön koşullar vardır:

- Desteklenen platformlar: Windows 10 sürüm 1607 veya üstü (kurumsal, Pro ve eğitim sürümleri).
- Desteklenen mimari: x86 ve x64.
- Cihaz yönetimi: AAD katılmış ve otomatik kayıtlı (karma etki alanına katılmış ve Grup ilkesi otomatik olarak kayıtlı).
- Uygulama paketi biçimi:. [Microsoft Win32 Içerik Prep aracı](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)tarafından hazırlanan **intunewın** dosyası.
- Malar
    - Maksimum boyut: 8MM.
    - Desteklenmeyen mimari: kolları.

Bu adımlarla ilgili bilgiler için belgeyi "[Microsoft Intune 'Da Win32 uygulaması ekleme, atama ve izleme](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" bölümünü gözden geçirin.

Win32 uygulamaları da dahil olmak üzere Windows 'da uygulama dağıtımının sorunlarını giderme ile ilgili ayrıntılar aşağıdaki belgelerde incelenebilir

- [Uygulama yükleme sorunlarını giderme](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Win32 uygulamalarında sorun giderme](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)