---
title: Office güncelleştirmeleriyle birlikte yüklenmiş Teams
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
ms.openlocfilehash: 36b0b1a7bf37c27304b4124157dba9aba337678c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832402"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>Office güncelleştirmeleriyle birlikte yüklenmiş Microsoft Teams

Microsoft Teams; Kurumsal  Microsoft 365 Uygulamaları, İş için Microsoft 365 Uygulamaları ve Office Mac'in yeni yüklemelerinin bir parçası olarak dahil edilir. Daha fazla bilgi için [bkz. Microsoft Teams yeni Office yüklemelerine ne zaman dahil edilecek?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Ayrıca, Güncel Kanal'daki Sürüm 1906'dan itibaren  Teams, var olan kurulumlarınızı en son sürüme güncelleştirince Windows çalıştıran cihazlarda kuruluş için Microsoft 365 Uygulamaları'nın (ve İş için Microsoft 365 Uygulamalarının) mevcut yüklemelerine aşamalı olarak eklenecektir. Daha fazla bilgi için [bkz. Mevcut Office yüklemeleri hakkında ne?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Not:** Bu dağıtım zamanlaması için beklemek istemiyorsanız, bu yönergeleri izleyerek Teams'i [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)kullanıcılarınız için tek başına olarak dağıtabilirsiniz veya kullanıcılarınızı 'dan kendi başına Teams yüklemelerini https://teams.microsoft.com/downloads sebilirsiniz.

Organizasyonunız Teams'i dağıtmaya hazır değilse, ***Teams'i*** yeni veya mevcut Office [yüklemelerinin](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) dışında tutebilirsiniz. [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Teams'in yüklemesini istiyor, ancak yüklendikten sonra kullanıcı için Teams'in otomatik olarak başlamasını istemiyorsanız bkz. Microsoft Teams'in yüklemeden sonra otomatik [olarak başlamasını engelleme](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

***Teams'i Windows*** çalıştıran bir cihazdan kaldırmak için bkz. [Microsoft Teams'i kaldırma.](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81) Microsoft Teams'i birden çok hedef makineden veya kullanıcıdan temizlemek için [bkz. Microsoft Teams dağıtım temizleme](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Paylaşılan bilgisayarlar, Uzak Masaüstü Hizmetleri (RDS) veya Sanal Masaüstü Altyapısı (VDI) kullanıyorsanız bkz. Microsoft Teams ile paylaşılan bilgisayar ve [VDI ortamları.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams) Office Mac kullanıyorsanız bkz. [Mac'te Microsoft Teams yüklemeleri](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**Not:** Teams yüklendikten sonra, yeni özellikler ve [kalite güncelleştirmeleriyle](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) yaklaşık iki haftada bir otomatik olarak güncelleştirilir. 