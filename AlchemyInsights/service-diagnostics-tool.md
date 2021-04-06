---
title: Windows Sanal Masaüstü için hizmet tanılama aracı
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596044"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="6bd3e-102">Windows Sanal Masaüstü için hizmet tanılama aracı</span><span class="sxs-lookup"><span data-stu-id="6bd3e-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="6bd3e-103">Windows Sanal Masaüstü (WVD), yöneticilerin hataları tek bir arabirim üzerinden tanımlamalarına olanak sağlayan bir tanılama aracı sunar.</span><span class="sxs-lookup"><span data-stu-id="6bd3e-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="6bd3e-104">Bu araç, WVD rolü atanan biri tarafından her WVD kullanılasında tanılamayla ilgili bilgileri günlüğe kaydeder.</span><span class="sxs-lookup"><span data-stu-id="6bd3e-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="6bd3e-105">Her günlük, etkinlikte yer alan WVD rolü, oturum sırasında görünen hata iletileri ve kiracı ve kullanıcı hakkında bilgi içerir.</span><span class="sxs-lookup"><span data-stu-id="6bd3e-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="6bd3e-106">Azure Log Analytics, aşağıdaki adımlarla tanılama aracı tarafından oluşturulan etkinlik günlüğünü yakalamak üzere yalndırabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="6bd3e-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="6bd3e-107">[Azure portalı](https://go.microsoft.com/fwlink/?linkid=2129500) veya Azure PowerShell ile bir Log Analytics çalışma alanı [oluşturun.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="6bd3e-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="6bd3e-108">[Windows bilgisayarlarını Azure Monitor'e bağlama.](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="6bd3e-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="6bd3e-109">Çalışma alanı kimliğini ve çalışma alanı birincil anahtarını alırsınız.</span><span class="sxs-lookup"><span data-stu-id="6bd3e-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="6bd3e-110">Kurulum sihirbazı aracıyı düzgün bir şekilde yapılandırmak ve Azure Monitor ile iletişim kuraya sahip olduğundan emin olmak için bu bilgiye gerekmektedir.</span><span class="sxs-lookup"><span data-stu-id="6bd3e-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="6bd3e-111">[Tanılama verilerini çalışma alanınıza bastırın.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="6bd3e-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="6bd3e-112">Tanılama verilerini WVD kiracıdan çalışma alanınız için Log Analytics'e İtebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6bd3e-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="6bd3e-113">WVD [ile](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) ilişkili olarak iç veya dış sorunları tanılar ve tanılar.</span><span class="sxs-lookup"><span data-stu-id="6bd3e-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="6bd3e-114">WVD için hizmet tanılama aracını yapılandırma hakkında daha fazla bilgi edinmek için bkz. Tanılama özelliği için Log Analytics'i kullanma.</span><span class="sxs-lookup"><span data-stu-id="6bd3e-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>