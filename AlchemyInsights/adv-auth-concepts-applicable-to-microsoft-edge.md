---
title: Microsoft Edge için geçerli olan gelişmiş kimlik doğrulama kavramları
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573780"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="a3c5a-102">Microsoft Edge için geçerli olan gelişmiş kimlik doğrulama kavramları</span><span class="sxs-lookup"><span data-stu-id="a3c5a-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="a3c5a-103">Microsoft Edge için geçerli olan gelişmiş kimlik doğrulama kavramları aşağıda verilmiştir:</span><span class="sxs-lookup"><span data-stu-id="a3c5a-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="a3c5a-104">**Önleyici kimlik doğrulama**</span><span class="sxs-lookup"><span data-stu-id="a3c5a-104">**Proactive Authentication**</span></span>

<span data-ttu-id="a3c5a-105">[Proactiveauthenabled](https://go.microsoft.com/fwlink/?linkid=2134621) ilkesini etkinleştirdiğinizde, Microsoft Edge, oturumu açık kullanıcılarla Microsoft hizmetlerini kullanarak kimlik doğrulama yapmayı dener.</span><span class="sxs-lookup"><span data-stu-id="a3c5a-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="a3c5a-106">Düzenli aralıklarla, önleyici kimlik doğrulamayı yöneten yapılandırmayı içeren güncelleştirilmiş bir bildirimi denetlemek için bir çevrimiçi hizmet kullanacaktır.</span><span class="sxs-lookup"><span data-stu-id="a3c5a-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="a3c5a-107">Yararlar: önleyici kimlik doğrulaması, Office yeni sekme sayfası gibi temel hizmetlerin kimlik doğrulamasını sağlar.</span><span class="sxs-lookup"><span data-stu-id="a3c5a-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="a3c5a-108">Ayrıca, Bing arama altyapısı olarak kullanılırsa, önleyici kimlik doğrulaması, adres çubuğunun performansını artırır ve işinizin ihtiyaçlarına göre kişiselleştirilmiş arama sonuçlarının oluşturulmasına yardımcı olur.</span><span class="sxs-lookup"><span data-stu-id="a3c5a-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="a3c5a-109">**NTLM kimlik doğrulaması için Windows Hello Creduı**</span><span class="sxs-lookup"><span data-stu-id="a3c5a-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="a3c5a-110">Web sitesi NTLM veya anlaşma mekanizması aracılığıyla Kullanıcı oturum açmaya çalıştığında çoklu oturum açma (SSO) kullanılamıyorsa, bu özellik kullanıcının işletim sistemi kimlik bilgilerini Web sitesiyle paylaşmasına ve Windows Hello Credentials Kullanıcı arabirimini kullanarak kimlik doğrulama sınamasını sağlamasına olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="a3c5a-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="a3c5a-111">Bu oturum açma akışı yalnızca Windows 10 ' da, yalnızca NTLM veya anlaşma sırasında SSO kullanmayan kullanıcılar için görünür.</span><span class="sxs-lookup"><span data-stu-id="a3c5a-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="a3c5a-112">**Otomatik olarak oturum açmak için kaydedilmiş parolaları kullanma**</span><span class="sxs-lookup"><span data-stu-id="a3c5a-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="a3c5a-113">Microsoft Edge 'de parolaları kaydeden kullanıcılar, kimlik bilgilerini kaydetdikleri web sitelerinde otomatik oturum açmayı etkinleştirebilirler.</span><span class="sxs-lookup"><span data-stu-id="a3c5a-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="a3c5a-114">Kullanıcılar edge://settings/passwords 'da bu özelliği açıp kapatabilir ve bunu [Parola Yöneticisi](https://go.microsoft.com/fwlink/?linkid=2134622) ilkelerinde yapılandırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a3c5a-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
