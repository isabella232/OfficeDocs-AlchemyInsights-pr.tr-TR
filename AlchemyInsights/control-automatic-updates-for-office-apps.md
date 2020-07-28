---
title: Office Uygulamaları için otomatik güncelleştirmeleri denetleme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439928"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="a59d3-102">Office Uygulamaları için otomatik güncelleştirmeleri denetleme</span><span class="sxs-lookup"><span data-stu-id="a59d3-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="a59d3-103">Varsayılan olarak, Office Apps güncelleştirmeleri otomatik olarak indirilir ve herhangi bir kullanıcı müdahalesi olmadan arka planda uygulanır.</span><span class="sxs-lookup"><span data-stu-id="a59d3-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="a59d3-104">Ancak yöneticiler, Office Update ayarlarını kullanarak güncelleştirmelerin nasıl uygulandığını denetleyebilir.</span><span class="sxs-lookup"><span data-stu-id="a59d3-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="a59d3-105">Güncelleştirme ayarları, yöneticilerin otomatik güncelleştirmeleri etkinleştirmesine veya devre dışı bırakarak Office'te **Şimdi Güncelleştir** düğmesini göstermesine veya gizlemesine, güncelleştirme son tarihlerini ayarlamasına ve daha fazlasını sağlamasına olanak tanır.</span><span class="sxs-lookup"><span data-stu-id="a59d3-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="a59d3-106">Ayrıntılı bilgi için bkz:</span><span class="sxs-lookup"><span data-stu-id="a59d3-106">For detailed information, see:</span></span>

- [<span data-ttu-id="a59d3-107">Office için güncelleştirme ayarlarını yapılandırma</span><span class="sxs-lookup"><span data-stu-id="a59d3-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="a59d3-108">Office için otomatik güncelleştirme etkinleştirildi</span><span class="sxs-lookup"><span data-stu-id="a59d3-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="a59d3-109">Office yüklendikten sonra nasıl güncelleştirin</span><span class="sxs-lookup"><span data-stu-id="a59d3-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="a59d3-110">İstemci makinesine uygulanan varolan güncelleştirme ayarlarını gözden geçirmek için aşağıdaki adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="a59d3-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="a59d3-111">**Başlat**  >  **Çalıştır**  >  **regedit'e**giderek Kayıt Defteri Düzenleyicisini açın.</span><span class="sxs-lookup"><span data-stu-id="a59d3-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="a59d3-112">Aşağıdaki konuma geçin ve Office Güncelleştirmesi ayarlarını gözden geçirin:</span><span class="sxs-lookup"><span data-stu-id="a59d3-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="a59d3-113">a.</span><span class="sxs-lookup"><span data-stu-id="a59d3-113">a.</span></span> <span data-ttu-id="a59d3-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="a59d3-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="a59d3-115">b.</span><span class="sxs-lookup"><span data-stu-id="a59d3-115">b.</span></span> <span data-ttu-id="a59d3-116">ClickToRun\Yapılandırma</span><span class="sxs-lookup"><span data-stu-id="a59d3-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="a59d3-117">**Not**  OfficeMgmtCOM anahtarı ayarlanmışsa, **Office**  >  **Hesap**  >  **Ofisi Güncelleştirmeleri'nde**"Güncelleştirmeler sistem yöneticiniz tarafından yönetilir" iletisini görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a59d3-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="a59d3-118">Daha fazla bilgi için Microsoft [Endpoint Configuration Manager ile Microsoft 365 Uygulamalarındaki güncelleştirmeleri yönet'e](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)bakın.</span><span class="sxs-lookup"><span data-stu-id="a59d3-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  