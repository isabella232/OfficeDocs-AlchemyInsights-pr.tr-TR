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
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401927"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="f876a-102">Hibrit Microsoft Azure AD katılımı sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="f876a-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="f876a-103">Kesinlikle Önerilir [Cihaz Kaydı Bağlantısını Test Et betiğini](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) kullanarak bir cihazın sistem hesabı altındaki Cihaz kaydı uç noktalarına erişebildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="f876a-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="f876a-104">Cihaz kayıtlarını ilk kez ayarlıyorsanız, Microsoft Azure AD denetimindeki cihazlara nasıl erişeceğinizi öğrenmek için [Azure Active Directory’de cihaz yönetimine giriş](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) makalesini incelemeyi unutmayın.</span><span class="sxs-lookup"><span data-stu-id="f876a-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="f876a-105">Cihazları doğrudan Microsoft Azure AD’ye kaydediyor ve bunları Intune’a kaydediyorsanız, ilk olarak [Intune’u yapılandırmayı](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ve [lisans](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) edinmeyi unutmayın. </span><span class="sxs-lookup"><span data-stu-id="f876a-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="f876a-106">Microsoft Azure AD’de ve şirket içi AD’de işlem yapma yetkiniz olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="f876a-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="f876a-107">Microsoft Azure AD’de yalnızca bir genel yönetici cihaz kayıtlarıyla ilgili ayarları yönetebilir.</span><span class="sxs-lookup"><span data-stu-id="f876a-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="f876a-108">Ek olarak, şirket içi Active Directory’de otomatik kayıtlar ayarlıyorsanız, (mümkünse) Active Directory ve AD FS yöneticisi olmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="f876a-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="f876a-109">Hibrit katılımla ilgili olası sorunları çözme konusunda daha fazla ayrıntı için bkz. [Hibrit Katılım Sorunlarını Giderme](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Hibrit Azure AD ile katılan ayarlama ve Microsoft Azure AD portalını kullanarak Cihazları Yönetme için bkz. [Hibrit Azure AD ile katılan (şirket içi etki alanına katılmış) cihazlar ayarlama](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) ve [Azure portal aracılığıyla cihazları yönetme](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f876a-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="f876a-110">Hibrit Azure Active Directory (AD) katılımıyla ilgili yaygın sorunları çözmek için bkz. [Hibrit Azure Active Directory katılımıyla ilgili SSS](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="f876a-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
