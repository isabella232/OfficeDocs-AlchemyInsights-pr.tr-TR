---
title: Ekipleri bağımsız veya yeni veya varolan Office yüklemeleriyle dağıtma
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 5ec5277a758fc5171c846266787c2fbcf751f21c
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617915"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Ekipleri bağımsız veya yeni veya varolan Office yüklemeleriyle dağıtma

Microsoft Teams artık Microsoft 365 Apps kurumsal, Microsoft 365 Apps iş için uygulamalar ve Mac için ***Office'in yeni yüklemelerinin*** bir parçası olarak eklenmiştir. Daha fazla bilgi için bkz: [Microsoft Ekipleri Yeni Office yüklemelerine ne zaman eklenmeye başlar?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Ayrıca, Geçerli Kanal'da Sürüm 1906'dan başlayarak, Mevcut yüklemenizi en son sürüme güncellediğinizde Windows çalıştıran cihazlardaki Microsoft 365 Apps kurumsal (ve iş için Microsoft 365 Apps) ***mevcut yüklemelerine takımlar eklenir.*** Daha fazla bilgi için [bkz.](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Bu kullanıma alma zamanlamasını beklemek istemiyorsanız, [bu yönergeleri izleyerek](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)ekiplerinizi kullanıcılarınız için tek başına   dağıtabilir veya kullanıcılarınızın Takımlar'ı kendileri için yüklemesini sağlayabilirsiniz.  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)

Kuruluşunuz Takımlar dağıtmaya hazır değilse, Ekipleri [yeni](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) veya [varolan](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office yüklemelerinden ***hariç tutmak*** için atabileceğiniz adımlara sahibiz. Takımlar'ın yüklenmesini, ancak ekiplerin yüklendikten sonra kullanıcı için otomatik olarak başlatılmasını istemiyorsanız, microsoft [ekiplerinin yüklemeden sonra otomatik olarak başlatılmasını engelleyin'](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)e bakın.

Windows çalıştıran bir aygıttan ***Takımlar kaldırmak*** için Microsoft [Ekiplerini](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)Kaldır'ı'na bakın. Microsoft Ekiplerini birden çok hedef makineden veya kullanıcıdan temizlemek için Microsoft [Teams dağıtımının temizlenmesine](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)bakın.

Paylaşılan bilgisayarları, Uzak Masaüstü Hizmetlerini (RDS) veya Sanal Masaüstü Altyapısı (VDI) kullanıyorsanız, [Microsoft Teams ile paylaşılan bilgisayar ve VDI ortamlarına](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)bakın.

Mac için Office kullanıyorsanız, [Mac'teki Microsoft Teams yüklemelerine](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)bakın.

> [!NOTE]
> Takımlar yüklendikten sonra, yeni özellikler ve kalite güncelleştirmeleriyle yaklaşık iki haftada bir [otomatik olarak güncellenir.](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) 