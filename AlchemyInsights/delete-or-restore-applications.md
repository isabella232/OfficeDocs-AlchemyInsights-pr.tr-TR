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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015021"
---
# <a name="delete-or-restore-applications"></a>Uygulamaları silme veya geri yükleme

**Azure AD kiracınızdaki bir uygulamayı silmek için**:

1. **Azure AD portalında** **Kurumsal uygulamalar**'ı seçin. Ardından, silmek istediğiniz uygulamayı bulun ve seçin.
2. Sol bölmedeki **Yönet** bölümünde **Özellikler**'i seçin.
3. **Sil**'i seçin ve Azure AD kiracınızdaki uygulamayı silmek istediğinizi onaylamak Için **Evet 'i** seçin.

Uygulamayı silme hakkında daha fazla bilgi için, [hızlı başlangıç: Azure Active Directory (Azure AD) kiracınızdaki bir uygulamayı silme](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

PowerShell 'de, [Remove-Azureadapplicationproxyapma](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet 'ı Azure Active Directory 'de belirli bir uygulamadan uygulama proxy yapılandırmalarını kaldırır ve belirtilmişse uygulamayı tamamen silebilir.

**Silinmiş bir uygulamayı PowerShell kullanarak geri yükleyebilirsiniz** . Geri yüklemek istediğiniz uygulama tanımlandıktan sonra, [restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)kullanarak geri yükleyebilirsiniz.
