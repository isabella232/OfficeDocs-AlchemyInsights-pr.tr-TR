---
title: Tek Teams olarak ya da yeni veya var olan kullanıcı yüklemeleriyle Office dağıtma
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
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102222"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Tek Teams olarak ya da yeni veya var olan kullanıcı yüklemeleriyle Office dağıtma

Microsoft Teams artık Yeni Kurulum,  Kurulum, Kurulum ve Kurulum Kurumlar için Microsoft 365 Uygulamaları İş için Microsoft 365 Uygulamaları bir Office Mac. Daha fazla bilgi için [bkz. Microsoft Teams yeni kurulumlara ne zaman dahil Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Buna ek olarak, Güncel Kanal'daki Sürüm 1906'dan başlayarak Teams, var olan yüklemenizi en son sürüme güncelleştirinca Windows çalıştıran cihazlardaki Kurumlar için Microsoft 365 Uygulamaları (ve İş için Microsoft 365 Uygulamaları) mevcut yüklemelerine de eklenecektir.  Daha fazla bilgi için [bkz. Mevcut Yüklemeler hakkında Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Bu dağıtım zamanlaması için beklemek istemiyorsanız, bu yönergeleri izleyerek Teams'yi kullanıcılarınız için tek başına dağıtabilirsiniz veya kullanıcılarınızı 'dan kendi Teams [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) yükleyebilirsiniz. [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)

Organizasyonunız dağıtıma hazır değilse Teams yeni veya var olan kullanıcı yüklemelerinin dışında tutmak [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) Teams [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) adımlar Office.  Yüklemenin Teams istiyor, ancak kullanıcı için Teams yüklendikten sonra otomatik olarak başlatmasını istemiyorsanız bkz. [Yüklemeden](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)sonra Microsoft Teams'in otomatik olarak başlamasını engelleme .

***E-Teams*** çalıştıran bir cihazdan Windows için bkz. [Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Birden çok Microsoft Teams makineden veya kullanıcıdan temizleme işlemi yapmak için [bkz. Microsoft Teams temizleme](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Paylaşılan bilgisayarlar, Uzak Masaüstü Hizmetleri (RDS) veya Sanal Masaüstü Altyapısı (VDI) kullanıyorsanız bkz. Paylaşılan bilgisayar ve [VDI](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)ortamları Microsoft Teams.

Office Mac kullanıyorsanız bkz. Mac [Microsoft Teams yüklemeleri yükleme](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Yeni Teams yüklendikten sonra, yeni [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) özellikler ve kalite güncelleştirmeleri ile yaklaşık her iki haftada bir otomatik olarak güncelleştirilir. 