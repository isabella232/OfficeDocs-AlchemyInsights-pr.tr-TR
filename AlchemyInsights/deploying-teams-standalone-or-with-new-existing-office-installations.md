---
title: Takımlar olarak tek başına veya yeni veya varolan Office yüklemeleri dağıtma
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054250"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Takımlar olarak tek başına veya yeni veya varolan Office yüklemeleri dağıtma

Microsoft Teams olan şimdi Mac için Office 365 ProPlus, Office 365 iş ve Office ***Yeni yüklemeler*** bir parçası olarak dahil Daha fazla bilgi için bkz: [ne zaman Microsoft Teams başlayacak yeni Office yüklemelerini eklenmesini?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Ayrıca, sürüm 1906 aylık kanal içinde başlayarak, takımlar ***eklediğiniz varolan yüklemeler için*** Office 365 ProPlus (ve Office 365 Business), varolan bir yükleme en son sürüme güncelleştirdiğinizde, Windows çalıştıran aygıtlarda olacaktır. Daha fazla bilgi için bkz: [Varolan Office yüklemelerini nasıldır?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Bu ürün zamanlama için beklemek istemiyorsanız, takımlar bağımsız, kullanıcılar için [Bu yönergeleri takip](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)ederek dağıtabilirsiniz veya kullanıcılarınızın takımlar kendileri için yüklemek olabilir [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Kuruluşunuzun takımlar dağıtmaya hazır değilse, [Yeni](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) veya [Varolan](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office yüklemelerinden ***Dışla ekipler*** için atabileceğiniz adımlar sahibiz. Ekiplerin yüklenmesi, ancak yok yüklendikten sonra kullanıcı için otomatik olarak başlatmak için takımlar istiyor, bkz: [Microsoft ekipleri yüklemeden sonra otomatik olarak başlatılmasını engellemek](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)istiyorsanız.

***Takımlar kaldırmak*** için Windows çalıştıran bir aygıttan, [Microsoft ekipleri kaldırma](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)konusuna bakın. Birden çok hedef makineler veya kullanıcılar temizleme Microsoft Teams için [Microsoft ekipleri dağıtım temizleme](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)konusuna bakın.

Paylaşılan bir bilgisayar kullanıyorsanız, Uzak Masaüstü Hizmetleri (RDS) veya Sanal Masaüstü Altyapısı (VDI) bkz: [paylaşılan bilgisayar ve Microsoft ekipleri ile VDI ortamlar](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Mac için Office kullanıyorsanız, [Mac Microsoft ekipleri yüklemelerinde](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)bakın.

> [!NOTE]
> Takımlar yüklendikten sonra [otomatik olarak](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) yaklaşık iki haftada yeni özellikler ve güncelleştirmeler kalitesi ile güncelleştirilmiştir. 