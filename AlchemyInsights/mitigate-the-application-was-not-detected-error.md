---
title: Uygulama algılanmadı hatasını azaltma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810503"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="769f2-102">"Uygulama algılanmadı" hatasını azaltma</span><span class="sxs-lookup"><span data-stu-id="769f2-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="769f2-103">Intune tarafından bildirilen uygulama yükleme hatası “Yükleme başarıyla tamamlandıktan sonra uygulama algılanmadı” tüm önemli işletim sistemi platformlarında (Windows, iOS ve Android) oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="769f2-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="769f2-104">Bu hatayı oluşturan en yaygın senaryolar şunlardır:</span><span class="sxs-lookup"><span data-stu-id="769f2-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="769f2-105">İlk dağıtımdan sonra uygulama Intune’un dışında güncelleştirildi (üçüncü taraf bir uygulama mağazasından).</span><span class="sxs-lookup"><span data-stu-id="769f2-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="769f2-106">Örneğin Google Chrome gibi bazı uygulamalar otomatik güncelleştirmeler yapabilir.</span><span class="sxs-lookup"><span data-stu-id="769f2-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="769f2-107">İlk yüklemeden sonra kullanıcı uygulamayı kaldırdı.</span><span class="sxs-lookup"><span data-stu-id="769f2-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="769f2-108">Bu sorunu azaltmak için önce etkilenen cihazları gözden geçirip hatanın oluştuğu senaryoyu saptayın.</span><span class="sxs-lookup"><span data-stu-id="769f2-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="769f2-109">Uygulama Intune’un dışında güncelleştirildiyse, uygulama dağıtımı uygulama sürümünü yoksayacak şekilde ayarlanabilir.</span><span class="sxs-lookup"><span data-stu-id="769f2-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="769f2-110">Bunu yapmak için **Uygulama Yapılandırması > Uygulama Bilgileri**’nin altında **Uygulama sürümünü yoksay** seçeneğini **Evet** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="769f2-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="769f2-111">İstemciyi hedeflerken uygulamayı “gerekli” olarak dağıtmak ve en son sürümün dağıtıldığından emin olmak uygun olabilir.</span><span class="sxs-lookup"><span data-stu-id="769f2-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="769f2-112">Alternatif olarak, işletim sistemi platformunda Apple Volume Purchase Program ile ilişkilendirilmiş **autoupdate** işlevselliğini kullanmak mümkündür. Bu, kullanıma sunulan yeni uygulama sürümlerine otomatik güncelleştirme yapılacak şekilde yapılandırılabilir.</span><span class="sxs-lookup"><span data-stu-id="769f2-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="769f2-113">Uygulama yükleme sorunlarını giderme hakkında daha fazla bilgi için bkz. [Uygulama yükleme sorunlarını giderme](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="769f2-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
