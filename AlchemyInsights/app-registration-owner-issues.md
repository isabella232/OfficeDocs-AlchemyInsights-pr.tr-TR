---
title: Uygulama Kayıt Sahibi sorunları
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405324"
---
# <a name="app-registration-owner-issues"></a>Uygulama Kayıt Sahibi sorunları

Aşağıda, uygulama kayıtlarda sorumluları sahip olarak eklemenin kullanılabilir yöntemleri yer almaktadır:

- Azure AD PowerShell Modülünü Kullanma -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Başvuru: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Azure CLI kullanma - `az ad app owner add`

    Başvuru: [az reklam uygulaması sahibi](https://docs.microsoft.com/cli/azure/ad/app/owner)
- MS Graph'i kullanma -

    Başvuru: [Sahip ekleme - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Azure AD Portalını kullanma - Portal.azure.com [>](https://portal.azure.com/) Azure Active directory > Uygulama Kaydı'> > Sahipler > Ekle'yi seçin

**Uygulamanın sahibi sizseniz bile uygulama kayıtlarda görüntülene misiniz?**

Uygulamanın sahibi yönetim rolü değildir. [Azure AD yönetim portalına](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) erişimi kısıtla ayarı etkinleştirilirse, uygulama kayıt portalında uygulamaları yalnızca yönetici ilebilir. Bir sahibin uygulamaları görüntüley olması için, bu ayarı devre dışı bırak (Bunu HAYıR olarak ayarla) veya yönetici rolünü yalnızca belirli bir uygulamanın sahibine attayabilirsiniz. Ancak bunun için Azure AD Premium P2 lisansına sahip olmak ve Ayrıcalıklı Kimlik Yönetimi'yi [etkinleştirmek gerekir.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
