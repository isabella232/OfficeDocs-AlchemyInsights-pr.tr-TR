---
title: Azure AD rolüne Grup atama
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
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885401"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="fd721-102">Azure AD rolüne Grup atama</span><span class="sxs-lookup"><span data-stu-id="fd721-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="fd721-103">Azure AD rolüne sahip bir Azure AD grubunu bir Azure AD rolüne atamak için aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="fd721-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="fd721-104">Yeni Grup oluşturma-yeni grup oluşturmak Için:</span><span class="sxs-lookup"><span data-stu-id="fd721-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="fd721-105">a.</span><span class="sxs-lookup"><span data-stu-id="fd721-105">a.</span></span> <span data-ttu-id="fd721-106">**Ayrıcalıklı rol yöneticisi** veya **genel yönetıcı** izinleriyle Azure AD Yönetim Merkezi 'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="fd721-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="fd721-107">b.</span><span class="sxs-lookup"><span data-stu-id="fd721-107">b.</span></span> <span data-ttu-id="fd721-108">**Tüm gruplar > yeni grup > Için Azure Active Directory > gruplar**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="fd721-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="fd721-109">c.</span><span class="sxs-lookup"><span data-stu-id="fd721-109">c.</span></span> <span data-ttu-id="fd721-110">Grubu oluşturun.</span><span class="sxs-lookup"><span data-stu-id="fd721-110">Create the group.</span></span>

2. <span data-ttu-id="fd721-111">Rolü Grup oluşturma sırasında veya Grup oluşturulduktan sonra gruba atayın.</span><span class="sxs-lookup"><span data-stu-id="fd721-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="fd721-112">a.</span><span class="sxs-lookup"><span data-stu-id="fd721-112">a.</span></span> <span data-ttu-id="fd721-113">Gruba, Grup oluşturma sırasında bir rol atamak için, **Azure AD rollerini Değiştir grubuna** ve grubu oluşturmaya geçebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="fd721-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="fd721-114">b.</span><span class="sxs-lookup"><span data-stu-id="fd721-114">b.</span></span> <span data-ttu-id="fd721-115">Oluşturulduktan sonra gruba rol atamak için, yeni oluşturulan grubun **atanan roller** sekmesine gidin ve rolü gruba atayın.</span><span class="sxs-lookup"><span data-stu-id="fd721-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="fd721-116">**Azure AD rolüne atanmış bir grubun üyeliğini yönetme**</span><span class="sxs-lookup"><span data-stu-id="fd721-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="fd721-117">Ayrıcalıkların yükseltilmesini önleyerek, varsayılan olarak yalnızca ayrıcalıklı rol yöneticileri ve genel Yöneticiler role atanmış bir grubun üyeliğini değiştirebilir.</span><span class="sxs-lookup"><span data-stu-id="fd721-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="fd721-118">Ancak, bu tür bir grubun sahibini atamayı seçebilir ve bu göreve temsilci atarsınız.</span><span class="sxs-lookup"><span data-stu-id="fd721-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="fd721-119">Azure AD rollerine bulut grupları atama hakkında daha fazla bilgi için bkz: [bulut grubuna ad rolleri atama](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="fd721-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="fd721-120">Bulut gruplarına atanan rollerle ilgili sorun giderme hakkında daha fazla bilgi için, [bulut gruplarına atanan rollerle Ilgili sorun giderme](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="fd721-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





