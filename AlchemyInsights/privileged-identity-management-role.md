---
title: Ayrıcalıklı kimlik yönetimi rolü
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089148"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="fc645-102">Ayrıcalıklı kimlik yönetimi (PıM) rolü</span><span class="sxs-lookup"><span data-stu-id="fc645-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="fc645-103">**Rol etkinleştirildikten sonra izinler verilmez**</span><span class="sxs-lookup"><span data-stu-id="fc645-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="fc645-104">Azure AD ayrıcalıklı kimlik yönetimi 'nde (PıM) bir rol etkinleştirdiğinizde, etkinleştirme ayrıcalıklı rol gerektiren tüm portallarına anında yaymayabilir.</span><span class="sxs-lookup"><span data-stu-id="fc645-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="fc645-105">Bazen, değişiklik yayılsa bile, portalda Web önbelleğe alma, değişikliğin hemen etkinleşmez.</span><span class="sxs-lookup"><span data-stu-id="fc645-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="fc645-106">Etkinleştirme gecikirse, şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="fc645-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="fc645-107">Azure portalında oturumu kapatın ve yeniden oturum açın.</span><span class="sxs-lookup"><span data-stu-id="fc645-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="fc645-108">Bir Azure AD rolünü veya bir Azure Kaynak rolünü etkinleştirdiğinizde, etkinleştirme aşamaları görüntülenir.</span><span class="sxs-lookup"><span data-stu-id="fc645-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="fc645-109">Tüm aşamalar tamamlandığında, ' oturumu Kapat ' bağlantısını görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="fc645-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="fc645-110">Oturumu kapatabilirsiniz. Bu, çoğu durumda etkinleştirme gecikmesini çözecektir.</span><span class="sxs-lookup"><span data-stu-id="fc645-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="fc645-111">PıM 'de, rolün üyesi olarak listelendiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="fc645-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="fc645-112">Exchange Yöneticisi rolünü etkinleştiriyorsanız, oturumunuzu kapatıp yeniden oturum açın.</span><span class="sxs-lookup"><span data-stu-id="fc645-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="fc645-113">Sorun devam ederse, bir destek bileti açın ve bunu sorun olarak yükseltin.</span><span class="sxs-lookup"><span data-stu-id="fc645-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="fc645-114">Güvenlik ve Uyumluluk Merkezi 'ne erişmek için Exchange Yöneticisi rolünü kullanıyorsanız, sonraki adıma bakın.</span><span class="sxs-lookup"><span data-stu-id="fc645-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="fc645-115">Güvenlik ve Uyumluluk Merkezi 'ne erişmek için bir rol etkinleştiriyorsanız veya SharePoint Yöneticisi rolünü etkinleştiriyorsanız, birkaç dakikadan birkaç saat kadar birkaç etkinleştirme gecikmeyle karşılaşırsınız.</span><span class="sxs-lookup"><span data-stu-id="fc645-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="fc645-116">Bu bilinen bir sorundur ve bu ekiple en kısa sürede bu sorunu çözmek için etkin bir şekilde çalışmaktadır.</span><span class="sxs-lookup"><span data-stu-id="fc645-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="fc645-117">Daha fazla bilgi için bkz.:</span><span class="sxs-lookup"><span data-stu-id="fc645-117">For more information, see:</span></span>

- [<span data-ttu-id="fc645-118">PıM 'de Azure AD rollerimi etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="fc645-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="fc645-119">PıM 'de Azure Resource rollerimi etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="fc645-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="fc645-120">**Rolün etkinliğini kaldırdıktan sonra izinler kaldırılmıyor veya rol etkinleştirme süresi dolarsa**</span><span class="sxs-lookup"><span data-stu-id="fc645-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="fc645-121">Azure AD ayrıcalıklı kimlik yönetimi 'nde bir rolün etkinliğini kaldırdığınızda veya bir rol etkinleştirme dönemi sona erdiğinde, erişime sahip olduğunuz bir gecikme olabilir.</span><span class="sxs-lookup"><span data-stu-id="fc645-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="fc645-122">Devre dışı bırakma işlemi gecikirse, şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="fc645-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="fc645-123">Exchange Yöneticisi rolünü devre dışı bırakırsanız veya rol etkinleştirme dönemi sona erdiğinde, bir destek bileti açın ve Office 'in sahip olduğu ayrıcalıklı erişim yönetimi (PAM) ekibiyle bir bilet dosyalarınıza yardımcı olmak için destek mühendisinizden yardım alın.</span><span class="sxs-lookup"><span data-stu-id="fc645-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="fc645-124">Etkinleştirme süresi dolduysa, ancak hala tarayıcı oturumu açıksa tarayıcınızı kapatın.</span><span class="sxs-lookup"><span data-stu-id="fc645-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="fc645-125">Bu oturumu kapatana kadar rolü kullanmaya devam edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fc645-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="fc645-126">Bu bilinen bir sorundur ve etkinleştirmenin süresi dolduğunda oturumu etkin bir şekilde iptal etmek için olası bir düzeltmeye bakıyoruz.</span><span class="sxs-lookup"><span data-stu-id="fc645-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="fc645-127">Gecikme bu iki senaryodan farklıysa lütfen bir destek bileti açın.</span><span class="sxs-lookup"><span data-stu-id="fc645-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
