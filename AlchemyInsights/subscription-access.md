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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999260"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Tarayıcı sorunları nedeniyle Azure'da oturum açamıyor (Tarayıcı askıda, dönen devam ediyor, yük vermiyor vb.)

Kesinti sizi etkiliyor olabilir. Devam eden bir kesinti olup olduğunu görmek için lütfen kontrol edin: [Azure Health Status](https://status.azure.com/status/history/).

Lütfen tüm etkin Azure oturumlarının oturumlarını out out. Web tarayıcınızın özel veya gizli modunu başlatın.

Ayrıca Tarayıcıyı yenilemeyi, başka bir tarayıcı kullanmayı, yukarıdaki işe yaramadı mı önbellek tanımlama bilgilerini silmeyi de deneyebilirsiniz.

Daha fazla bilgi: [Oturum açma sorunlarını giderme](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Abonelikler erişemiyor**

Azure [portalında,](https://portal.azure.com/)sağ üst hesaptan doğru Azure dizininin seçildiğinden emin olun.

Azure [Hesap merkezi'nde,](https://account.windowsazure.com/Subscriptions)kullanılan hesabın hesap yöneticisi olup olduğundan emin olun.

Daha fazla bilgi edinin: [Abonelik bulunamadı sorunlarını giderme](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ödeme geçmişine erişilamadı**

Hesap yöneticisinin fatura bilgilerine erişen kullanıcının Azure Active Directory'ye konuk kullanıcı olarak eklendiklarından emin olması [gerekir: Yeni](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)kullanıcı ekleme veya silme .

Bundan sonra kullanıcıya bir Genel yönetici rolü atanmalı: [Kullanıcılara rol atama](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Bunu yayınla, kullanıcıya RBAC ilkeleri kullanılarak faturalama erişimi verilmiştir: [Faturalandırmaya erişim izni ver](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Önerilen Belgeler**

-   [Azure aboneliğimi yönetmek için oturum alikme](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)