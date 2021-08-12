---
title: Hibrit Microsoft Azure AD katılımı sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939291"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Hibrit Microsoft Azure AD katılımı sorunlarını giderme

Kesinlikle Önerilir [Cihaz Kaydı Bağlantısını Test Et betiğini](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) kullanarak bir cihazın sistem hesabı altındaki Cihaz kaydı uç noktalarına erişebildiğinden emin olun.

1. Cihaz kayıtlarını ilk kez ayarlıyorsanız, Microsoft Azure AD denetimindeki cihazlara nasıl erişeceğinizi öğrenmek için [Azure Active Directory’de cihaz yönetimine giriş](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) makalesini incelemeyi unutmayın.
1. Cihazları doğrudan Microsoft Azure AD’ye kaydediyor ve bunları Intune’a kaydediyorsanız, ilk olarak [Intune’u yapılandırmayı](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ve [lisans](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) edinmeyi unutmayın. 
1. Microsoft Azure AD’de ve şirket içi AD’de işlem yapma yetkiniz olduğundan emin olun. Microsoft Azure AD’de yalnızca bir genel yönetici cihaz kayıtlarıyla ilgili ayarları yönetebilir. Ek olarak, şirket içi Active Directory’de otomatik kayıtlar ayarlıyorsanız, (mümkünse) Active Directory ve AD FS yöneticisi olmanız gerekir.

Hibrit katılımla ilgili olası sorunları çözme konusunda daha fazla ayrıntı için bkz. [Hibrit Katılım Sorunlarını Giderme](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Hibrit Azure AD ile katılan ayarlama ve Microsoft Azure AD portalını kullanarak Cihazları Yönetme için bkz. [Hibrit Azure AD ile katılan (şirket içi etki alanına katılmış) cihazlar ayarlama](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) ve [Azure portal aracılığıyla cihazları yönetme](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Hibrit Azure Active Directory (AD) katılımıyla ilgili yaygın sorunları çözmek için bkz. [Hibrit Azure Active Directory katılımıyla ilgili SSS](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
