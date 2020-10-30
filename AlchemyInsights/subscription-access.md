---
title: Abonelik erişimi
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807725"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Tarayıcı sorunları nedeniyle Azure 'da oturum açılamıyor (tarayıcı kilitleniyor, dönmeyi sürdürür, yüklenmiyor, yüklenmiyor vb.)

Bir kesinti olabilir. Devam eden bir kesinti olup olmadığını denetleyin: [Azure uygunluk durumu](https://status.azure.com/status/history/).

Lütfen tüm etkin Azure oturumlarından oturum açın. Web tarayıcınızın özel veya tam bir modunu başlatma.

Ayrıca, tarayıcıyı yenilemeyi deneyebilir, başka bir tarayıcı kullanabilir, yukarıdaki durumlarda önbellek tanımlama bilgilerini silebilirsiniz.

Daha fazla bilgi: [oturum açma sorunlarını giderme](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Aboneliklere erişilemiyor**

[Azure portalında](https://portal.azure.com/), sağ üstteki hesaptan doğru Azure dizininin seçildiğinden emin olun.

[Azure Hesap Merkezi](https://account.windowsazure.com/Subscriptions)'nde, kullanılan hesabın hesap yöneticisi olduğundan emin olun.

[Abonelik bulunamayan sorun giderme](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Fatura geçmişine erişilemiyor**

Hesap yöneticisinin, fatura bilgilerine erişen kullanıcının, Azure Active Directory 'ye Konuk Kullanıcı olarak eklendiğinden emin olması gerekmektedir: [Yeni Kullanıcı ekleme veya silme](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Ardından kullanıcıya genel yönetici rolü verilmelidir: [kullanıcılara rol atayın](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Bunu gönder: kullanıcıya RBAC ilkeleri kullanılarak faturalandırma erişimi verilebilir: [faturalandırma için erişim Izni verme](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Önerilen belgeler**

-   [Azure aboneliğimi yönetmek için oturum açamıyorum](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)