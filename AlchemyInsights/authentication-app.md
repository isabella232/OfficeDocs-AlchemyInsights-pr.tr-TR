---
title: Kimlik doğrulama uygulaması
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
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405684"
---
# <a name="authentication-app"></a><span data-ttu-id="25adf-102">Kimlik doğrulama uygulaması</span><span class="sxs-lookup"><span data-stu-id="25adf-102">Authentication app</span></span>

<span data-ttu-id="25adf-103">Genel Yöneticiyseniz Oturum Açma Tanılama'yı kullanarak kullanıcı oturum açmayla ilgili ne olduğunu hemen bulabilir veya sorunları [tanıabilirsiniz.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="25adf-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="25adf-104">Tanılamayı başlatmak için "Tanılamayı[Başlat"](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)düğmesine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="25adf-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="25adf-105">Kullanıcı, uygulama, oturum açma zamanı, kimlik isteği veya bağıntı kimliği hakkında sahip olduğunuz ayrıntıları girerek analiz etmek için olayı bulun.</span><span class="sxs-lookup"><span data-stu-id="25adf-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="25adf-106">Ne olduğunu ve gerekirse değişiklik yapmak için hangi eylemleri gerçekleştirebilirsiniz ayrıntılarını gösteren tanılama sonuçlarını gözden geçirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="25adf-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="25adf-107">**Uygun olan senaryoyu kontrol edin:**</span><span class="sxs-lookup"><span data-stu-id="25adf-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="25adf-108">Kullanıcı Microsoft Authenticator uygulamasında bir anında bildirim alsa bile, Engelleme ve kullanıcıların engellemesini kaldırma konusunda açıklandığı gibi MFA engellenen kullanıcıların altında [gösterilmeyebileceklerini doğrulayın.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="25adf-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="25adf-109">Kullanıcı MFA için engellenmiş ancak bir anında bildirim almayacaksa, Microsoft Authenticator uygulamasını açabilir ve bu da bekleyen onay isteklerini çeker.</span><span class="sxs-lookup"><span data-stu-id="25adf-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="25adf-110">Alternatif bir oturum açma yöntemi olarak, kullanıcı başka bir yolla Oturum aç'a tıklar ve mobil uygulamamdan bir doğrulama kodu kullanmayı seçebilir.</span><span class="sxs-lookup"><span data-stu-id="25adf-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="25adf-111">Microsoft Authenticator Uygulaması, birçok kullanıcı için kullanılabilen tek yöntemdir.</span><span class="sxs-lookup"><span data-stu-id="25adf-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="25adf-112">[Güvenlik varsayılanları hakkında daha fazla bilgi edinin,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) [Authenticator Uygulaması hakkında sık](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) sorulan sorular ve bunları çözme hakkında SSS bölümünü inceleyin.</span><span class="sxs-lookup"><span data-stu-id="25adf-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="25adf-113">**Önerilen Videolar**</span><span class="sxs-lookup"><span data-stu-id="25adf-113">**Recommended Videos**</span></span>

<span data-ttu-id="25adf-114">[Authenticator Uygulamasını yeni bir telefonda (2 dakika) ayarlama.](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="25adf-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
