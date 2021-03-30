---
title: Azure Active Directory'ye katılma
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405669"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="3a52a-102">Azure Active Directory'ye katılma</span><span class="sxs-lookup"><span data-stu-id="3a52a-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="3a52a-103">Cihaz kayıtlarını ilk kez ayarıyorsanız, Cihazları Azure AD'de denetim altına alma hakkında size yol sağlayacak [Azure Active Directory'de](/azure/active-directory/devices/overview) cihaz yönetimine giriş'i gözden geçirmeyi gözden geçirmeyi öğrenin.</span><span class="sxs-lookup"><span data-stu-id="3a52a-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="3a52a-104">Cihazları doğrudan Azure AD'ye kaydedecek ve bunları Intune'a kaydedeceksanız, [önce Intune'u](/mem/intune/enrollment/device-enrollment) yapılandırmış ve lisansa sahip olduğunuzdan emin olun. [](/mem/intune/fundamentals/licenses-assign)</span><span class="sxs-lookup"><span data-stu-id="3a52a-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="3a52a-105">Azure AD'de işlem gerçekleştirmek için yetkiniz olduğundan emin olmak.</span><span class="sxs-lookup"><span data-stu-id="3a52a-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="3a52a-106">Cihaz kayıtlarının ayarlarını yalnızca Azure AD'de genel yönetici yönetebilir.</span><span class="sxs-lookup"><span data-stu-id="3a52a-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="3a52a-107">Azure AD'ye katılma uygulamasını yapmak için Bkz. [Azure AD Katılma Planı.](/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="3a52a-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="3a52a-108">Azure AD katılmayla ilgili sık karşılaşılan sorunları çözme hakkında daha fazla ayrıntı için Azure [Ad Join](/azure/active-directory/devices/faq) SSS'ye bakın ve Windows 10 pro cihazı için bkz. [Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)makinesi Azure AD'ye katılamıyor - Yükseltme gerekiyor - Microsoft Topluluğu.</span><span class="sxs-lookup"><span data-stu-id="3a52a-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
