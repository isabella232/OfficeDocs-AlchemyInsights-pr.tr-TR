---
title: Bağlantılar ve URL 'Ler ile ilgili sorunlar
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974757"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="18d08-102">Bağlantılar ve URL 'Ler ile ilgili sorunlar</span><span class="sxs-lookup"><span data-stu-id="18d08-102">Issues with links and URLs</span></span>

<span data-ttu-id="18d08-103">URI/Reply URL 'Lerini yeniden yönlendir (her iki ifade da her iki ifade da değiştirilebilir), uygulama tarafından istenen belirteçleri döndürmek için Microsoft Identity platform tarafından kullanılan URL 'Ler</span><span class="sxs-lookup"><span data-stu-id="18d08-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="18d08-104">Bu URL 'Ler hakkında bilgi için aşağıdaki makalelere bakın:</span><span class="sxs-lookup"><span data-stu-id="18d08-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="18d08-105">[Kimlik doğrulama akışları ve uygulama senaryoları](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) -her senaryonun **uygulama kaydı** sayfasında yeniden yönlendirme URI 'leri hakkında bilgi.</span><span class="sxs-lookup"><span data-stu-id="18d08-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="18d08-106">Yönlendirme URI 'SI/yanıt URL kısıtlamaları ve sınırlamaları</span><span class="sxs-lookup"><span data-stu-id="18d08-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="18d08-107">**Uygulamam için RIGHT Redirect URI/Reply URL 'sini nasıl kaydedeceğinizi bilmiyorum**</span><span class="sxs-lookup"><span data-stu-id="18d08-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="18d08-108">Geliştirdiğiniz uygulama ile oturum açtığınızda, oturum açma iletişim kutusu **AADSTS50011 görüntülüyorsa: istekte belirtilen yanıt URL 'si uygulama <your app ID> için yapılandırılmış olan yanıt URL 'leriyle eşleşmezse**, uygulama kaydınızı, kod isteğinde kodunuzun Microsoft Identity platformuna KULLANDıĞı yeniden yönlendirme URI 'sini de eklemeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="18d08-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="18d08-109">Bir yanıt URL 'SI eklemek için, Azure portalında **uygulama kayıt** sayfanızda **kimlik doğrulama** sekmesine gidin ve **Uri 'leri yönlendir** bölümüne bir girdi ekleyin.</span><span class="sxs-lookup"><span data-stu-id="18d08-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="18d08-110">Yönlendirme URI 'Leri yazılır (Web veya mobil/masaüstü).</span><span class="sxs-lookup"><span data-stu-id="18d08-110">Redirect URIs are typed (Web or mobile/desktop).</span></span> <span data-ttu-id="18d08-111">Girmeniz gereken değer, aşağıda açıklandığı gibi, oluşturduğunuz uygulama türüne bağlıdır:</span><span class="sxs-lookup"><span data-stu-id="18d08-111">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="18d08-112">Tek sayfalık uygulamalar ve Web uygulamaları için, yanıt URL 'SI uygulamanızdaki bir URL olur.</span><span class="sxs-lookup"><span data-stu-id="18d08-112">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="18d08-113">Azure portalını kullanarak [tek sayfalı uygulama kaydı](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) veya [Web uygulaması uygulaması kaydettirme](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="18d08-113">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="18d08-114">Masaüstü uygulamaları için, seçmeniz gereken değer aşağıdakilere bağlıdır:</span><span class="sxs-lookup"><span data-stu-id="18d08-114">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="18d08-115">Platform (MacOS, Windows veya Linux 'tan farklıdır)</span><span class="sxs-lookup"><span data-stu-id="18d08-115">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="18d08-116">Bu belirteci edinme yöntemi (etkileşimli olarak, tümleşik Windows kimlik doğrulaması [ıWA] veya Kullanıcı adı/parola ile).</span><span class="sxs-lookup"><span data-stu-id="18d08-116">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="18d08-117">Ayrıntılar için bkz: [Masaüstü uygulamaları-App Registration-Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="18d08-117">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="18d08-118">Mobil uygulamalar için, yönlendirme URI 'SI aşağıdakilere bağlıdır:</span><span class="sxs-lookup"><span data-stu-id="18d08-118">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="18d08-119">Platform (iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="18d08-119">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="18d08-120">iOS 'daki paket KIMLIĞI ve Android 'deki paket adı ve imza karması gibi uygulamanızı oluşturmak için kullanılan bilgiler, Azure portal uygulaması kaydı size yardımcı olacaktır.</span><span class="sxs-lookup"><span data-stu-id="18d08-120">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="18d08-121">Ayrıntılar için [, bkz.](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="18d08-121">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="18d08-122">Web API 'Leri ve belirteçleri (ıWA ve kullanıcıadı/parola) almanın sessiz yollarından bazıları yeniden yönlendirme URI 'SI gerektirmez.</span><span class="sxs-lookup"><span data-stu-id="18d08-122">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="18d08-123">**Web uygulamamı Kuruluşum ve Dağıtılmış uygulamayı sındığımda, yanıt URL uyumsuzluğu iletisi alıyorum**</span><span class="sxs-lookup"><span data-stu-id="18d08-123">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="18d08-124">Web uygulamanızı dağıttığınız tüm konumlar için yeniden yönlendirme URI 'Leri ekleyin.</span><span class="sxs-lookup"><span data-stu-id="18d08-124">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="18d08-125">Daha fazla bilgi için bkz [.](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)</span><span class="sxs-lookup"><span data-stu-id="18d08-125">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="18d08-126">Uygulamayı bu konumda dağıttıktan hemen sonra bir konum için yeniden yönlendirme URI 'SI ekleyin.</span><span class="sxs-lookup"><span data-stu-id="18d08-126">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="18d08-127">**Yeterli yanıt URL 'Lerini kaydedemiyorum**</span><span class="sxs-lookup"><span data-stu-id="18d08-127">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="18d08-128">Bir ISV kullanıyorsunuz ve size ait her müşteri için bir veya birkaç yeniden yönlendirme Uri 'si vardır.</span><span class="sxs-lookup"><span data-stu-id="18d08-128">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="18d08-129">ADAL/Azure AD v 1.0'dan MSAL/Microsoft Identity platformuna geçirmek istiyorsunuz ve [yeniden yönlendirme URI sayısı üst sınırına](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris)ulaşıldı.</span><span class="sxs-lookup"><span data-stu-id="18d08-129">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="18d08-130">Bunu çözmek için, müşterilerinize [yönlendirilen URI 'leri hizmet sorumlularına ekleyin](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) .</span><span class="sxs-lookup"><span data-stu-id="18d08-130">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
