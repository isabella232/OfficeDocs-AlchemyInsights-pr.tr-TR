---
title: Windows sanal masaüstü için Azure portalını kullanarak uygulama gruplarını yönetme
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
- "9003956"
- "7013"
ms.openlocfilehash: 0dd08d04ad6328e7afa158b36517839fc31a8566
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722052"
---
# <a name="manage-app-groups-by-using-the-azure-portal-for-windows-virtual-desktop"></a><span data-ttu-id="6a3d8-102">Windows sanal masaüstü için Azure portalını kullanarak uygulama gruplarını yönetme</span><span class="sxs-lookup"><span data-stu-id="6a3d8-102">Manage app groups by using the Azure portal for Windows Virtual Desktop</span></span>

<span data-ttu-id="6a3d8-103">Yeni Windows sanal masaüstü konak havuzu için oluşturulan varsayılan uygulama grubu, tam masaüstünü de yayımlar.</span><span class="sxs-lookup"><span data-stu-id="6a3d8-103">The default app group created for a new Windows Virtual Desktop host pool also publishes the full desktop.</span></span> <span data-ttu-id="6a3d8-104">Ayrıca, Azure Portal 'ı kullanmak, konak havuzu için bir veya daha fazla RemoteApp uygulaması grubu oluşturmanıza olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="6a3d8-104">In addition, using the Azure portal lets you create one or more RemoteApp app groups for the host pool.</span></span>

<span data-ttu-id="6a3d8-105">Dağıtım işlemi aşağıdakileri yapacak:</span><span class="sxs-lookup"><span data-stu-id="6a3d8-105">The deployment process will do the following:</span></span>

1. <span data-ttu-id="6a3d8-106">RemoteApp uygulama grubu oluşturun.</span><span class="sxs-lookup"><span data-stu-id="6a3d8-106">Create the RemoteApp app group.</span></span>
2. <span data-ttu-id="6a3d8-107">Seçilen uygulamalarınızı uygulama grubuna ekleyin.</span><span class="sxs-lookup"><span data-stu-id="6a3d8-107">Add your selected apps to the app group.</span></span>
3. <span data-ttu-id="6a3d8-108">Tek tek kullanıcıları veya Kullanıcı gruplarını uygulama grubuna yayımlayın.</span><span class="sxs-lookup"><span data-stu-id="6a3d8-108">Publish individual users or user groups to the app group.</span></span>
4. <span data-ttu-id="6a3d8-109">Bunu yapmak isterseniz uygulama grubunu kaydettirin.</span><span class="sxs-lookup"><span data-stu-id="6a3d8-109">Register the app group, if you choose to do so.</span></span>
5. <span data-ttu-id="6a3d8-110">Yapılandırmanıza göre Azure Resource Manager şablonuna yönelik bir bağlantı oluşturun; böylece indirebilir ve kaydedebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6a3d8-110">Create a link to an Azure Resource Manager template according to your configuration, which you can download and save.</span></span>

<span data-ttu-id="6a3d8-111">Windows sanal masaüstü için RemoteApp grubu oluşturmak üzere, [Azure portalında uygulama gruplarını yönetme](https://go.microsoft.com/fwlink/?linkid=2129550)bölümündeki yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="6a3d8-111">To create a RemoteApp group for Windows Virtual Desktop, follow the instructions in [Manage app groups with the Azure portal](https://go.microsoft.com/fwlink/?linkid=2129550).</span></span>
