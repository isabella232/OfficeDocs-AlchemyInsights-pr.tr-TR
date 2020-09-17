---
title: Ekipleri tek başına veya yeni veya mevcut Office yüklemeleriyle dağıtma
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
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806779"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Ekipleri tek başına veya yeni veya mevcut Office yüklemeleriyle dağıtma

Microsoft ekipleri kurumsal olarak Microsoft 365 uygulamalarının kurumsal, Microsoft 365 iş ve Mac için Office uygulamalarının ***Yeni yüklemelerinin*** bir parçası olarak eklenmiştir. Daha fazla bilgi için [Microsoft ekipleri yeni Office yüklemelerine ne zaman eklenecek?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Ayrıca, geçerli kanaldaki 1906 sürümünden başlayarak, mevcut yüklemenizi en son sürüme güncelleştirdiğinizde Windows çalıştıran cihazlarda kurumsal (ve Microsoft 365 uygulamaları için Microsoft uygulamaları) ***kurulumlarının mevcut 365 yüklemelerine eklenir*** . Daha fazla bilgi için [Office 'in var olan yüklemelerinde ne var?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Bu kademeli bir zamanlama için beklemek istemezseniz, [Bu yönergeleri Izleyerek](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)ekiplerinizi kullanıcılarınız için tek başına dağıtabilirsiniz   veya kullanıcılarınızın kendilerinin kendilerine takımları yüklemesini sağlayabilirsiniz  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Kuruluşunuz ekipleri dağıtmaya hazır değilse, [Yeni](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) veya [mevcut](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office yüklemelerinden ***ekip dışında tutmak*** için uygulayabileceğiniz adımlara sahip olabiliriz. Ekiplerin yüklenmesini istiyorsanız, ancak ekipten sonra kullanıcıya otomatik olarak başlamasını istemiyorsanız, [yükleme sonrasında Microsoft ekiplerin otomatik olarak başlatılmasını önleyin](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Windows çalıştıran bir cihazdan ***ekipleri kaldırmak*** Için [Microsoft ekipleri kaldırma](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)konusuna bakın. Microsoft ekiplerini birden çok hedef makineden veya kullanıcılardan temizlemek için, bkz: [Microsoft ekipleri dağıtımı Temizleme](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Paylaşılan bilgisayarlar, Uzak Masaüstü Hizmetleri (RDS) veya sanal masaüstü altyapısı (VDı) kullanıyorsanız, [Microsoft ekipleri Ile paylaşılan bilgisayar ve VDI ortamları](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)'na bakın.

Mac için Office kullanıyorsanız, [Mac Için Microsoft ekipleri yüklemeleri](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)konusuna bakın.

> [!NOTE]
> Takımlar yüklendikten sonra, yeni özellikler ve kalite güncelleştirmeleriyle birlikte yaklaşık iki haftada bir [otomatik olarak güncelleştirilir](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) . 