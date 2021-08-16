---
title: Teams güncelleştirmeleriyle birlikte Office yükleme
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
- "2599"
- "9000140"
- "9000660"
- "2509"
ms.openlocfilehash: c473a001d1441362baad9feb44323b46f1cef42d3c431ef87f0fb0172f10d152
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048752"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>Microsoft Teams güncelleştirmeleriyle birlikte Office yüklü

Microsoft Teams, Kurulum, Kurulum ve  Kurulum Kurumlar için Microsoft 365 Uygulamaları İş için Microsoft 365 Uygulamaları bir Office Mac. Daha fazla bilgi için [bkz. Microsoft Teams yeni kurulumlara ne zaman dahil Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Buna ek olarak, Güncel Kanal'daki Sürüm 1906'dan başlayarak Teams, var olan yüklemenizi en son sürüme güncelleştirebilirsiniz ve Windows çalıştıran cihazlardaki mevcut Kurumlar için Microsoft 365 Uygulamaları (ve İş için Microsoft 365 Uygulamaları) yüklemelerine aşamalı olarak eklenecektir.  Daha fazla bilgi için [bkz. Mevcut Yüklemeler hakkında Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Not:** Bu dağıtım zamanlaması için beklemek istemiyorsanız, bu yönergeleri izleyerek Teams'yi kullanıcılarınız [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)için tek başına dağıtabilirsiniz veya kullanıcılarınızı 'dan kendileri için Teams https://teams.microsoft.com/downloads yükleyebilirsiniz.

Organizasyonunız dağıtıma hazır değilse Teams veya var ***olan*** Teams [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) yüklemelerini, bu dağıtımların yeni veya var olan yüklemelerinin dışında Office. [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Yüklemenin Teams istiyor, ancak kullanıcı için Teams yüklendikten sonra otomatik olarak başlatmasını istemiyorsanız bkz. [Yüklemeden](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)sonra Microsoft Teams'in otomatik olarak başlamasını engelleme .

***E-Teams*** çalıştıran bir cihazdan Windows için bkz. [Microsoft Teams.](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81) Birden çok Microsoft Teams makineden veya kullanıcıdan iş temizlemek için [bkz. Microsoft Teams temizleme.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Paylaşılan bilgisayarlar, Uzak Masaüstü Hizmetleri (RDS) veya Sanal Masaüstü Altyapısı (VDI) kullanıyorsanız bkz. Paylaşılan bilgisayar ve [VDI](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)ortamları Microsoft Teams. Office Mac kullanıyorsanız bkz. Mac [Microsoft Teams yüklemeleri yükleme](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**Not:** Yeni Teams yüklendikten sonra, yeni [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) özellikler ve kalite güncelleştirmeleri ile yaklaşık her iki haftada bir otomatik olarak güncelleştirilir. 