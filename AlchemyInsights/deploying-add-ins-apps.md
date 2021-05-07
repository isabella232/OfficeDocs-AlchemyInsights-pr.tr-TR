---
title: Eklentiler için eklentileri Microsoft 365 Uygulamaları
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233554"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Eklentiler için eklentileri Microsoft 365 Uygulamaları

Merkezi Dağıtım, eklentilerin, kuruluş içindeki kullanıcılara Office dağıtımı için önerilen yoldur. Eklentileri dağıtmak için aşağıdaki adımları izleyin:

**Not:** Kullanıcılara eklentileri yüklemek Office için bkz. Office programlarında [eklentileri görüntüleme, yönetme Office yükleme.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Ayrıca, Mağaza eklentilerinin ayrı Office satın alımının etkinleştirildiğinden emin olun. Ayrıntılar için [bkz. tüm istemcilerde Office Store'Office indirmelerini](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)engelleme (Outlook).

1. Merkezi Dağıtım kullanarak ortamının eklentilerin dağıtımıyla ilgili gereksinimleri karşı olduğundan emin olun. Ayrıntılar için bkz. [Gereksinimler](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Tümleştirilmiş **Ayarlar**  >  **Eklentilerin** dağıtımı  >  **için** Microsoft 365 Yönetim Merkezinde Uygulamaları edinin'e gidin. 

Notlar: 

- Tümleşik Uygulamalar için yöneticinin Genel Yönetici veya Yönetici Exchange olması gerekir.

- Eklentileri birden çok kullanıcıya dağıtırken, tek tek kullanıcılar yerine grupları kullanarak atamalar yapmalarını öneririz. Ayrıntılar için [bkz. Kullanıcılara ve gruplara eklenti atarken dikkate alınacak noktalar](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).

- Merkezi Dağıtım, iç içe gruplarda veya üst grupları olan gruplarda bulunan kullanıcıları desteklemez. Ayrıntılar için [bkz. Kullanıcı ve grup atamaları](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).

- Kullanıcıların oturum açması için Microsoft 365 Uygulama Yönetim Hizmeti'nin (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') etkinleştirildiğinden emin olun. Ayrıntılar için [bkz. Uygulama özelliklerini yapılandırma.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Tümleşik Uygulamaları kullanarak eklentilerin dağıtımında sorun yaşanıyorsa, Eklentileri kullanarak [dağıtmayı deneyin.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Daha fazla bilgi için bkz.:

[Yönetim merkezinde eklentileri dağıtma](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Yönetim merkezinde eklentileri yönetme](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Eklentileri yönetmek için Merkezi Dağıtım PowerShell cmdlet'lerini kullanma](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Yönetim Office Merkezi Dağıtım kullanarak Eklentileri Yayımlama Microsoft 365 yayımlama](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Sorun giderme: Kullanıcı eklentileri görmüyor](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Eklentilerle kullanıcı Office sorunlarını giderme](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)