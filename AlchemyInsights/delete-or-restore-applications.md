---
title: Uygulamaları silme veya geri yükleme
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102591"
---
# <a name="delete-or-restore-applications"></a>Uygulamaları silme veya geri yükleme

**Azure AD kiracıdan uygulama silmek için:**

1. Azure **AD portalında ,** diğer **Enterprise seçin.** Ardından silmek istediğiniz uygulamayı bulup seçin.
2. Sol **bölmede** bulunan Yönet bölümünde Özellikler'i **seçin.**
3. **Sil'i** seçin ve ardından **Azure AD** kiracıdan uygulama silmek istediğiniz onaylamak için Evet'i seçin.

Uygulama silme hakkında daha fazla bilgi için bkz. Hızlı Başlangıç: Azure Active Directory [(Azure AD) kiracıdan uygulama silme](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

PowerShell'de, [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet'i Azure Active Directory'te belirli bir uygulamanın Uygulama Ara Sunucusu yapılandırmalarını kaldırır ve belirtilirse uygulamayı tamamen silebilir.

PowerShell **kullanarak silinmiş bir uygulamayı** geri yükleyebilirsiniz. Geri yüklemek istediğiniz uygulama tanımlandıktan sonra, [Restore-AzureADDeletedApplication uygulamasını kullanarak geri yükleyebilirsiniz.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
