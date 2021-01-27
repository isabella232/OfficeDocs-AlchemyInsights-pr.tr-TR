---
title: Koşullu erişim sorunları
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015005"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="2fb3c-102">Koşullu erişim sorunları</span><span class="sxs-lookup"><span data-stu-id="2fb3c-102">Conditional access issues</span></span>

<span data-ttu-id="2fb3c-103">**Oturum açma tanısı sorunlarını çözme**</span><span class="sxs-lookup"><span data-stu-id="2fb3c-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="2fb3c-104">[Oturum açma tanılaması](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)kullanarak Kullanıcı oturum açma ile ilgili sorunları hızla bulabilir veya tanılayabilir:</span><span class="sxs-lookup"><span data-stu-id="2fb3c-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="2fb3c-105">Oturum açma tanılaması 'nı başlatın.</span><span class="sxs-lookup"><span data-stu-id="2fb3c-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="2fb3c-106">Kullanıcı, uygulama, oturum açma süresi, istek kimliği veya bağıntı kimliği hakkında sahip olduğunuz ayrıntılara girerek çözümlenecek olayı bulun.</span><span class="sxs-lookup"><span data-stu-id="2fb3c-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="2fb3c-107">Ne olduğunu ve değişiklik yapmak için uygulayabileceğiniz eylemleri (herhangi bir değişiklik gerekiyorsa) gösteren Tanılama sonuçlarını gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="2fb3c-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="2fb3c-108">**Oturum açma sorunlarını giderme adımları**</span><span class="sxs-lookup"><span data-stu-id="2fb3c-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="2fb3c-109">Azure AD oturum açma sayfasına gidin.</span><span class="sxs-lookup"><span data-stu-id="2fb3c-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="2fb3c-110">Oturum açmayı kullanıcıya, zaman aralığına, uygulamaya, duruma, istemci uygulamasına, vb. göre filtreleyin.</span><span class="sxs-lookup"><span data-stu-id="2fb3c-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="2fb3c-111">Hangi ilkelerin değerlendirildiğini görmek için bir oturum açma olayı seçin ve koşullu erişim sekmesini görüntüleyin.</span><span class="sxs-lookup"><span data-stu-id="2fb3c-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="2fb3c-112">İlke ayrıntılarını görüntülemek ve neden uygulandığını anlamak için bir ilkenin satırına tıklayın.</span><span class="sxs-lookup"><span data-stu-id="2fb3c-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="2fb3c-113">**Koşullu erişim ilkesinde sorun giderme araçları**</span><span class="sxs-lookup"><span data-stu-id="2fb3c-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="2fb3c-114">Yalnızca rapor modu kullanıcıları etkilemeden bir ilkeyi değerlendirmenize olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="2fb3c-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="2fb3c-115">Durum aracı, oturum açma olaylarının hangi ilkelerin uygulanacağını görmenizi sağlar.</span><span class="sxs-lookup"><span data-stu-id="2fb3c-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="2fb3c-116">Öngörüler ve raporlama çalışma kitabı her ilkenin gerçek zamanlı etkisini gösterir.</span><span class="sxs-lookup"><span data-stu-id="2fb3c-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="2fb3c-117">**Temel koruma Ilkeleri**</span><span class="sxs-lookup"><span data-stu-id="2fb3c-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="2fb3c-118">Temel koruma ilkeleri kullanımdan kaldırıldı.</span><span class="sxs-lookup"><span data-stu-id="2fb3c-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="2fb3c-119">Artık zorlanmayacak ve Azure portalından yakında kaldırılacaktır.</span><span class="sxs-lookup"><span data-stu-id="2fb3c-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="2fb3c-120">[Güvenlik varsayılanlarını](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)etkinleştirmeyi öneririz.</span><span class="sxs-lookup"><span data-stu-id="2fb3c-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="2fb3c-121">Koşullu erişimle ilgili daha fazla bilgi için bkz.</span><span class="sxs-lookup"><span data-stu-id="2fb3c-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="2fb3c-122">[Azure Active Directory 'de koşullu erişim Için en iyi yöntemler](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Koşullu erişimde koşullar](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Koşullu erişimde denetimler](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Koşullu erişimde konumlar](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="2fb3c-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
