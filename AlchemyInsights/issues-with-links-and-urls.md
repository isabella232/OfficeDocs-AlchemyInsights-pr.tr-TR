---
title: Bağlantılar ve URL'lerle ilgili sorunlar
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707902"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="2eb03-102">Bağlantılar ve URL'lerle ilgili sorunlar</span><span class="sxs-lookup"><span data-stu-id="2eb03-102">Issues with links and URLs</span></span>

<span data-ttu-id="2eb03-103">Yönlendirme URI'si/yanıt URL'leri (her iki ifade de birbirinin yerine kullanılabilir) uygulamanın istediği belirteçleri geri döndürmek için Microsoft kimlik platformu tarafından kullanılan URL'lerdir.</span><span class="sxs-lookup"><span data-stu-id="2eb03-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="2eb03-104">Bu URL'ler hakkında bilgi için aşağıdaki makalelere bakabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="2eb03-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="2eb03-105">[Kimlik doğrulama akışları ve uygulama senaryoları](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Her senaryo için **Uygulama kaydı** sayfasındaki yönlendirme URI'leri hakkında bilgiler.</span><span class="sxs-lookup"><span data-stu-id="2eb03-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="2eb03-106">Yönlendirme URI'si/yanıt URL'leri kısıtlamaları ve sınırlamaları</span><span class="sxs-lookup"><span data-stu-id="2eb03-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="2eb03-107">**Uygulamam için doğru yönlendirme URI'si / yanıt URL'lerini nasıl kaydedeceğimi bilmiyorum**</span><span class="sxs-lookup"><span data-stu-id="2eb03-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="2eb03-108">Geliştirdiğiniz uygulamayla oturum açtığınızda oturum açma iletişim kutusu **AADSTS50011 gösteriyorsa: İstekte belirtilen yanıt URL'si, <your app ID>** adlı uygulamanız için yapılandırılmış URL'ler ile eşleşmiyor. Microsoft kimlik platformuna belirteç isteğinde kullanılan kodunuzun yeniden yönlendirme URI'sini uygulama kaydınıza eklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="2eb03-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="2eb03-109">Yanıt URL'si eklemek için, Azure portalda bulunan **uygulama kayıt** sayfasındaki **Kimlik Doğrulaması** sekmesine gidin ve **Yönlendirme URI'leri** bölümüne bir girdi ekleyin.</span><span class="sxs-lookup"><span data-stu-id="2eb03-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="2eb03-110">Girmeniz gereken değer, aşağıda açıklandığı gibi oluşturduğunuz uygulama türüne bağlıdır:</span><span class="sxs-lookup"><span data-stu-id="2eb03-110">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="2eb03-111">Tek sayfalı uygulamalar ve web uygulamaları için yanıt URL'si uygulamanızdaki bir URL'dir.</span><span class="sxs-lookup"><span data-stu-id="2eb03-111">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="2eb03-112">Bkz: [Tek sayfalı uygulama kaydı](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) veya [Azure portal kullanarak bir web uygulamasını kaydetme](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="2eb03-112">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="2eb03-113">Masaüstü uygulamalarınız için seçmeniz gereken değer şunlara bağlıdır:</span><span class="sxs-lookup"><span data-stu-id="2eb03-113">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="2eb03-114">platform (MacOS, Windows veya Linux'ten farklıdır)</span><span class="sxs-lookup"><span data-stu-id="2eb03-114">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="2eb03-115">belirteci edinme yönteminiz (etkileşimli olarak, cihaz kodu akışıyla, Tümleşik Windows Kimlik Doğrulaması [IWA] ile veya kullanıcı adı/parolayla).</span><span class="sxs-lookup"><span data-stu-id="2eb03-115">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="2eb03-116">Ayrıntılar için bkz: [Masaüstü uygulamaları - Uygulama kaydı - Yönlendirme URI'si](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="2eb03-116">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="2eb03-117">Mobil uygulamalar için yönlendirme URI'si şunlara bağlıdır:</span><span class="sxs-lookup"><span data-stu-id="2eb03-117">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="2eb03-118">platform (iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="2eb03-118">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="2eb03-119">iOS'taki paket kimliği, Android'deki paket adı ve imza karması gibi uygulamanızı oluşturmak için kullanılan bilgiler. Azure portal uygulaması kaydı size yardımcı olacaktır.</span><span class="sxs-lookup"><span data-stu-id="2eb03-119">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="2eb03-120">Ayrıntılar için bkz: [Platform yapılandırması ve yönlendirme URI'leri](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="2eb03-120">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="2eb03-121">Web API'leri ve belirteç almanın bazı sessiz yolları (IWA ve kullanıcı adı/parola) yönlendirme URI'si gerektirmez.</span><span class="sxs-lookup"><span data-stu-id="2eb03-121">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="2eb03-122">**Web uygulamamı dağıttım ve dağıtılan uygulamayı test ettiğimde, yanıt URL'sinin uymadığına yönelik mesaj alıyorum.**</span><span class="sxs-lookup"><span data-stu-id="2eb03-122">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="2eb03-123">Web uygulamanızı dağıttığınız tüm konumlar için yönlendirme URI'leri ekleyin.</span><span class="sxs-lookup"><span data-stu-id="2eb03-123">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="2eb03-124">Daha fazla bilgi için bkz: [Azure portal kullanarak bir web uygulamasını kaydetme](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span><span class="sxs-lookup"><span data-stu-id="2eb03-124">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="2eb03-125">Uygulamayı o konumda dağıttıktan hemen sonra yönlendirme URI'sini konum için ekleyin.</span><span class="sxs-lookup"><span data-stu-id="2eb03-125">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="2eb03-126">**Yeterli yanıt URL'si kaydedemiyorum**</span><span class="sxs-lookup"><span data-stu-id="2eb03-126">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="2eb03-127">Her müşteriniz için bir veya birkaç yönlendirme URI'sinizin olduğu bir bağımsız yazılım satıcısısınız.</span><span class="sxs-lookup"><span data-stu-id="2eb03-127">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="2eb03-128">ADAL/Azure Active Directory v1.0'dan MSAL/Microsoft kimlik platformuna geçirmek istiyorsunuz ve [en fazla yönlendirme URI'si sayısına ulaştınız](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="2eb03-128">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="2eb03-129">Bunu çözmek için her bir müşterinize karşılık gelen [hizmet ilkelerine yeniden yönlendirme URI'leri ekleyin.](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals)</span><span class="sxs-lookup"><span data-stu-id="2eb03-129">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
