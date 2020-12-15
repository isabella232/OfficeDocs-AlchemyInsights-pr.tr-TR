---
title: Windows sanal masaüstü için hizmet Tanılama Aracı
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680235"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="8ddfd-102">Windows sanal masaüstü için hizmet Tanılama Aracı</span><span class="sxs-lookup"><span data-stu-id="8ddfd-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="8ddfd-103">Windows sanal masaüstü (WVD), yöneticilerin hataları tek bir arabirim aracılığıyla belirlemesine olanak tanıyan bir tanılama aracı sunar.</span><span class="sxs-lookup"><span data-stu-id="8ddfd-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="8ddfd-104">Bu araç, WVD rolüne atanan bir kullanıcı tarafından WVD kullanıldığında tanılamaların ilgili bilgilerini günlüğe kaydeder.</span><span class="sxs-lookup"><span data-stu-id="8ddfd-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="8ddfd-105">Her günlükte, faaliyette yer alan WVD rolüyle ilgili bilgiler, oturum sırasında görünen hata mesajları ve kiracı ile Kullanıcı hakkındaki bilgiler yer alır.</span><span class="sxs-lookup"><span data-stu-id="8ddfd-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="8ddfd-106">Azure Log Analytics, tanılama aracı tarafından oluşturulan etkinlik günlüğünü yakalamak üzere yapılandırılabilir.</span><span class="sxs-lookup"><span data-stu-id="8ddfd-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="8ddfd-107">Bunu şu şekilde yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="8ddfd-107">Here's how:</span></span>

1. <span data-ttu-id="8ddfd-108">[Azure portalı](https://go.microsoft.com/fwlink/?linkid=2129500) veya [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)ile bir Log Analytics çalışma alanı oluşturun.</span><span class="sxs-lookup"><span data-stu-id="8ddfd-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="8ddfd-109">[Windows bilgisayarlarını Azure monitöre bağlama](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="8ddfd-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="8ddfd-110">Çalışma alanınızın KIMLIĞINI ve çalışma alanınızın birincil anahtarını edinin.</span><span class="sxs-lookup"><span data-stu-id="8ddfd-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="8ddfd-111">Kurulum Sihirbazı, aracıyı düzgün bir şekilde yapılandırmak ve Azure Monitor ile iletişim kurabildiğinden emin olmak için bu bilgiye ihtiyaç duyar.</span><span class="sxs-lookup"><span data-stu-id="8ddfd-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="8ddfd-112">[Tanılama verilerini çalışma alanınıza gönderin](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="8ddfd-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="8ddfd-113">WVD kiracınızdaki tanılama verilerini çalışma alanınızın günlük çözümlemelerini gönderebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8ddfd-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="8ddfd-114">WVD ile ilgili iç veya dış [sorunları tanımlayın ve tanılayın](https://go.microsoft.com/fwlink/?linkid=2128338) .</span><span class="sxs-lookup"><span data-stu-id="8ddfd-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="8ddfd-115">WVD için hizmet Tanılama Aracı 'nı yapılandırma hakkında daha fazla bilgi edinmek için, [Tanılama özelliği Için Günlük Analizi kullanma](https://go.microsoft.com/fwlink/?linkid=2128084)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="8ddfd-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
