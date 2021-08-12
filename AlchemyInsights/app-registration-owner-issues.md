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
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951153"
---
# <a name="app-registration-owner-issues"></a>Uygulama Kayıt Sahibi sorunları

Aşağıda, uygulama kayıtlarına sahip olarak sorumluları eklemek için kullanılabilen yöntemler ve ücretlerinden birini kullanabilirsiniz:

- Azure AD PowerShell Modülü Kullanma -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Başvuru: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Azure CLI kullanma - `az ad app owner add`

    Başvuru: [az reklam uygulama sahibi](https://docs.microsoft.com/cli/azure/ad/app/owner)
- MS Graph kullanma -

    Başvuru: [Sahip ekleme - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Azure AD Portalını kullanma - Portal.azure.com [>](https://portal.azure.com/) Azure Active Directory > Uygulama Kaydı'> Uygulama Sahibi > ve Sahip >'i seçin

**Uygulamanın sahibi olsanız bile uygulama Kayıt Blade'inde uygulamanızı görüntüleye miyesiniz?**

Uygulamanın sahibi yönetim rolü değildir. [Azure AD yönetim portalına erişimi](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) kısıtla ayarı etkinleştirilirse, uygulamaları yalnızca yönetici Uygulama Kaydı portalında ilebilir. Bir sahibin uygulamaları görüntüley olması için bu ayarı devre dışı bırakarak (Bunu HAYıR olarak ayarlayın) veya yalnızca belirli bir uygulamanın sahibine yönetici rolü attayabilirsiniz. Bununla birlikte, bunun için lisans Azure AD Premium P2 ve [etkinleştirmeniz Privileged Identity Management.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
