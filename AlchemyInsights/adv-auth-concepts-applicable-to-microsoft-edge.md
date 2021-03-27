---
title: Microsoft Edge için uygun gelişmiş kimlik doğrulama kavramları
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398605"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="7e6b5-102">Microsoft Edge için uygun gelişmiş kimlik doğrulama kavramları</span><span class="sxs-lookup"><span data-stu-id="7e6b5-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="7e6b5-103">Aşağıda, Microsoft Edge için geçerli olan gelişmiş kimlik doğrulama kavramları ve bilgileri ve bilgileri yermektedir:</span><span class="sxs-lookup"><span data-stu-id="7e6b5-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="7e6b5-104">**Proaktif Kimlik Doğrulama**</span><span class="sxs-lookup"><span data-stu-id="7e6b5-104">**Proactive Authentication**</span></span>

<span data-ttu-id="7e6b5-105">[ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) ilkeyi etkinleştirseniz, Microsoft Edge Microsoft hizmetleri aracılığıyla oturum açık kullanıcıların önceden kimlik doğrulamasını yapmaya çalışır.</span><span class="sxs-lookup"><span data-stu-id="7e6b5-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="7e6b5-106">Düzenli aralıklarla, Proaktif Kimlik Doğrulaması'nın geçerli olduğu yapılandırmayı içeren güncelleştirilmiş bir bildirim olup denetlemesi için çevrimiçi bir hizmet kullanır.</span><span class="sxs-lookup"><span data-stu-id="7e6b5-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="7e6b5-107">Avantajlar: Proaktif Kimlik Doğrulama, Office Yeni Sekme Sayfası gibi önemli hizmetlerde kimlik doğrulamayı sağlar.</span><span class="sxs-lookup"><span data-stu-id="7e6b5-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="7e6b5-108">Ayrıca, Bing arama motoru olarak kullanılıyorsa, Proaktif Kimlik Doğrulama adres çubuğunun performansını artırır ve işletmenizin ihtiyaçlarına göre kişiselleştirilmiş arama sonuçları üretmeye yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="7e6b5-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="7e6b5-109">**NTLM Kimlik Doğrulaması için Windows Hello CredUI**</span><span class="sxs-lookup"><span data-stu-id="7e6b5-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="7e6b5-110">Bir web sitesi NTLM veya Görüşme mekanizması aracılığıyla kullanıcıda oturum açmaya çalıştığında çoklu oturum açma (SSO) kullanılamıyorsa, bu özellik kullanıcının işletim sistemi kimlik bilgilerini web sitesiyle paylaşmasına ve Windows Hello Cred UI kullanarak kimlik doğrulama zorluklarını karşılamasına olanak sağlar.</span><span class="sxs-lookup"><span data-stu-id="7e6b5-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="7e6b5-111">Bu oturum açma akışı yalnızca Windows 10'da ve yalnızca NTLM veya Görüşme sırasında SSO almayan kullanıcılar için görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="7e6b5-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="7e6b5-112">**Kaydedilen parolaları kullanarak otomatik olarak oturum açma**</span><span class="sxs-lookup"><span data-stu-id="7e6b5-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="7e6b5-113">Microsoft Edge'de parolaları kaydeden kullanıcılar, kimlik bilgilerini kaydettilen web sitelerinde otomatik olarak oturum açma özelliğini etkinleştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7e6b5-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="7e6b5-114">Kullanıcılar bu özelliği aynı edge://settings/passwords veya devre dışı bırakır ve parola yöneticisi ilkelerde [yapılandırabilirsiniz.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="7e6b5-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
