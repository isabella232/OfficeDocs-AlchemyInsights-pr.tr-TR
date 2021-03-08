---
title: Parola günlükleri
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527774"
---
# <a name="password-logs"></a><span data-ttu-id="7e3ee-102">Parola günlükleri</span><span class="sxs-lookup"><span data-stu-id="7e3ee-102">Password logs</span></span>

<span data-ttu-id="7e3ee-103">**Parola sıfırlama denetim günlüklerine erişirken sorunm var**</span><span class="sxs-lookup"><span data-stu-id="7e3ee-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="7e3ee-104">Parola sıfırlama denetim günlüklerine erişimle ilgili sorunları gidermek için aşağıdaki adımı gerçekleştirin:</span><span class="sxs-lookup"><span data-stu-id="7e3ee-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="7e3ee-105">Denetim günlüklerini görüntüleme yetkinizin olduğundan emin olmak.</span><span class="sxs-lookup"><span data-stu-id="7e3ee-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="7e3ee-106">Yalnızca aşağıdaki roller yetkilidir:</span><span class="sxs-lookup"><span data-stu-id="7e3ee-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="7e3ee-107">Genel yönetici</span><span class="sxs-lookup"><span data-stu-id="7e3ee-107">Global administrator</span></span>
 - <span data-ttu-id="7e3ee-108">Güvenlik yöneticisi</span><span class="sxs-lookup"><span data-stu-id="7e3ee-108">Security administrator</span></span>
 - <span data-ttu-id="7e3ee-109">Güvenlik gözetmeni</span><span class="sxs-lookup"><span data-stu-id="7e3ee-109">Security reader</span></span>

<span data-ttu-id="7e3ee-110">**İlk dağıtıldığından itibaren tüm parola sıfırlama denetim olaylarını görmek istiyorum**</span><span class="sxs-lookup"><span data-stu-id="7e3ee-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="7e3ee-111">Son 30 günlük raporlarda 120.000'e kadar parola sıfırlama/kayıt olayları depolanır.</span><span class="sxs-lookup"><span data-stu-id="7e3ee-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="7e3ee-112">CSV'i indirirken kullanıcı arabirimi için bu üst sınır geçerlidir.</span><span class="sxs-lookup"><span data-stu-id="7e3ee-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="7e3ee-113">PowerShell aracılığıyla 1 milyon etkinlik kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="7e3ee-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="7e3ee-114">Daha fazla bilgi için aşağıdaki bağlantılara bakın:</span><span class="sxs-lookup"><span data-stu-id="7e3ee-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="7e3ee-115">Azure AD Raporları ve Etkinlikleri API'sini kullanarak self servis parola sıfırlama olayları</span><span class="sxs-lookup"><span data-stu-id="7e3ee-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="7e3ee-116">PowerShell ile parola sıfırlama kayıt olaylarını hızla indirme</span><span class="sxs-lookup"><span data-stu-id="7e3ee-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="7e3ee-117">**Parola sıfırlama raporlama özellikleri hakkında daha fazla bilgi almak istiyorum**</span><span class="sxs-lookup"><span data-stu-id="7e3ee-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="7e3ee-118">Kullanıcılar ve gruplar altındaki Azure AD parola sıfırlama denetim günlüklerine kimlerin kaydolup kaydolacı olduğunu veya Azure AD parola sıfırlama denetim **günlüklerini kontrol edin.**</span><span class="sxs-lookup"><span data-stu-id="7e3ee-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="7e3ee-119">Daha fazla bilgi için aşağıdaki bağlantılara bakın:</span><span class="sxs-lookup"><span data-stu-id="7e3ee-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="7e3ee-120">Parola sıfırlama raporlarına genel bakış</span><span class="sxs-lookup"><span data-stu-id="7e3ee-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="7e3ee-121">Azure portalda parola sıfırlama raporlarını görüntüleme</span><span class="sxs-lookup"><span data-stu-id="7e3ee-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="7e3ee-122">Azure AD Raporları ve Etkinlikleri API'sini kullanarak self servis parola sıfırlama olayları</span><span class="sxs-lookup"><span data-stu-id="7e3ee-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="7e3ee-123">PowerShell ile parola sıfırlama kayıt olaylarını hızla indirme</span><span class="sxs-lookup"><span data-stu-id="7e3ee-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


