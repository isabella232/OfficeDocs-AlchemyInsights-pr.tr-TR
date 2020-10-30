---
title: Abonelik erişimi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807725"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="209fe-102">Tarayıcı sorunları nedeniyle Azure 'da oturum açılamıyor (tarayıcı kilitleniyor, dönmeyi sürdürür, yüklenmiyor, yüklenmiyor vb.)</span><span class="sxs-lookup"><span data-stu-id="209fe-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="209fe-103">Bir kesinti olabilir.</span><span class="sxs-lookup"><span data-stu-id="209fe-103">You might be impacted by an outage.</span></span> <span data-ttu-id="209fe-104">Devam eden bir kesinti olup olmadığını denetleyin: [Azure uygunluk durumu](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="209fe-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="209fe-105">Lütfen tüm etkin Azure oturumlarından oturum açın.</span><span class="sxs-lookup"><span data-stu-id="209fe-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="209fe-106">Web tarayıcınızın özel veya tam bir modunu başlatma.</span><span class="sxs-lookup"><span data-stu-id="209fe-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="209fe-107">Ayrıca, tarayıcıyı yenilemeyi deneyebilir, başka bir tarayıcı kullanabilir, yukarıdaki durumlarda önbellek tanımlama bilgilerini silebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="209fe-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="209fe-108">Daha fazla bilgi: [oturum açma sorunlarını giderme](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="209fe-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="209fe-109">**Aboneliklere erişilemiyor**</span><span class="sxs-lookup"><span data-stu-id="209fe-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="209fe-110">[Azure portalında](https://portal.azure.com/), sağ üstteki hesaptan doğru Azure dizininin seçildiğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="209fe-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="209fe-111">[Azure Hesap Merkezi](https://account.windowsazure.com/Subscriptions)'nde, kullanılan hesabın hesap yöneticisi olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="209fe-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="209fe-112">[Abonelik bulunamayan sorun giderme](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="209fe-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="209fe-113">**Fatura geçmişine erişilemiyor**</span><span class="sxs-lookup"><span data-stu-id="209fe-113">**Unable to access billing history**</span></span>

<span data-ttu-id="209fe-114">Hesap yöneticisinin, fatura bilgilerine erişen kullanıcının, Azure Active Directory 'ye Konuk Kullanıcı olarak eklendiğinden emin olması gerekmektedir: [Yeni Kullanıcı ekleme veya silme](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="209fe-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="209fe-115">Ardından kullanıcıya genel yönetici rolü verilmelidir: [kullanıcılara rol atayın](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="209fe-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="209fe-116">Bunu gönder: kullanıcıya RBAC ilkeleri kullanılarak faturalandırma erişimi verilebilir: [faturalandırma için erişim Izni verme](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="209fe-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="209fe-117">**Önerilen belgeler**</span><span class="sxs-lookup"><span data-stu-id="209fe-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="209fe-118">Azure aboneliğimi yönetmek için oturum açamıyorum</span><span class="sxs-lookup"><span data-stu-id="209fe-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)