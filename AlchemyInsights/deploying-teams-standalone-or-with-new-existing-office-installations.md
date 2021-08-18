---
title: Tek Teams olarak veya yeni veya var olan kullanıcı yüklemeleriyle Office dağıtma
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320142"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Tek Teams olarak veya yeni veya var olan kullanıcı yüklemeleriyle Office dağıtma

Microsoft Teams artık Yeni Kurulum, Kurulum, Kurulum ve Kurulum Kurumlar için Microsoft 365 Uygulamaları İş için Microsoft 365 Uygulamaları bir Office Mac.  Daha fazla bilgi için [bkz. Microsoft Teams yüklemelerinin yeni yüklemelerine ne zaman dahil Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Ayrıca, Güncel Kanal'daki Sürüm 1906'dan başlayarak Teams, var olan yüklemenizi en son sürüme güncelleştirebilirsiniz ve Windows çalıştıran cihazlardaki Kurumlar için Microsoft 365 Uygulamaları (ve İş için Microsoft 365 Uygulamaları) yüklemelerine de eklenir.  Daha fazla bilgi için [bkz. Mevcut Yüklemeler hakkında Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Not:** Bu dağıtım zamanlaması için beklemek istemiyorsanız, bu yönergeleri izleyerek kullanıcılarınız için [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) Teams'i tek başına dağıtabilirsiniz veya kullanıcılarınızı 'dan kendileri için Teams [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) yükleyebilirsiniz.

Organizasyonun dağıtıma hazır değilse Teams yeni veya var olan kullanıcı yüklemelerinin dışında tutmak [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) Teams [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) adımlar Office.  Yükleme Teams istiyor, ancak kullanıcı için Teams yüklendikten sonra otomatik olarak başlatmasını istemiyorsanız bkz. Microsoft Teams yüklendikten sonra otomatik olarak [başlamasını engelleme](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Yükleme ***Teams*** cihazdan kaldırmak için Windows [Kaldırma'ya Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Birden çok Microsoft Teams makineden veya kullanıcıdan temizleme işlemi yapmak için [bkz. Microsoft Teams temizleme](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Paylaşılan bilgisayarlar, Uzak Masaüstü Hizmetleri (RDS) veya Sanal Masaüstü Altyapısı (VDI) kullanıyorsanız bkz. Paylaşılan bilgisayar ve [VDI](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)ortamları Microsoft Teams.

Office Mac kullanıyorsanız [bkz. Mac Microsoft Teams yüklemeleri yükleme](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**Not:** Teams yüklendikten sonra, yeni özellikler [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) ve kalite güncelleştirmeleri ile yaklaşık iki haftada bir otomatik olarak güncelleştirilir. 