---
title: Cihaz etiketlerini veya gruplarını oluşturma ve yönetme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731971"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="5e910-102">Cihaz etiketlerini veya gruplarını oluşturma ve yönetme</span><span class="sxs-lookup"><span data-stu-id="5e910-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="5e910-103">Mantıksal bir grup bağlantıları oluşturmak için cihazlara etiketler ekleyin.</span><span class="sxs-lookup"><span data-stu-id="5e910-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="5e910-104">Cihaz etiketleri ağa düzgün eşlemeyi destekler ve bağlam yakalamak ve bir olayın parçası olarak dinamik liste oluşturulmasını sağlamak için farklı etiketler eklemenizi sağlar.</span><span class="sxs-lookup"><span data-stu-id="5e910-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="5e910-105">Etiketler, Cihazlar liste görünümünde filtre olarak veya cihazları grupla için kullanılabilir.</span><span class="sxs-lookup"><span data-stu-id="5e910-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="5e910-106">Cihaz gruplama hakkında daha fazla bilgi için [bkz. Cihaz etiketlerini oluşturma ve yönetme.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="5e910-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="5e910-107">Cihazlara etiket eklemek için:</span><span class="sxs-lookup"><span data-stu-id="5e910-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="5e910-108">Portalı kullanma</span><span class="sxs-lookup"><span data-stu-id="5e910-108">Using the portal</span></span>

- <span data-ttu-id="5e910-109">Kayıt defteri anahtarı değerini ayarlama</span><span class="sxs-lookup"><span data-stu-id="5e910-109">Setting a registry key value</span></span>
 
<span data-ttu-id="5e910-110">**Not:** Etiketin cihaza eklenme zamanı ile cihaz listesinde ve cihaz sayfasında kullanılabilirliği arasında gecikme olabilir.</span><span class="sxs-lookup"><span data-stu-id="5e910-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="5e910-111">API kullanarak cihaz etiketleri eklemek için bkz. [Cihaz etiketleri API'sini ekleme veya kaldırma.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="5e910-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="5e910-112">Portalı kullanarak cihaz etiketlerini ekleme ve yönetme</span><span class="sxs-lookup"><span data-stu-id="5e910-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="5e910-113">Etiketleri yönetmek istediğiniz cihazı seçin.</span><span class="sxs-lookup"><span data-stu-id="5e910-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="5e910-114">Aşağıdaki görünümlerden herhangi birini kullanarak bir cihazı seçerek veya arayabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="5e910-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="5e910-115">**Güvenlik işlemleri panosu** Etkin uyarıları olan en üst cihazlar bölümünden cihazın adını seçin.</span><span class="sxs-lookup"><span data-stu-id="5e910-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="5e910-116">**Uyarılar sırası** - Uyarılar kuyruğundan cihaz simgesinin yanındaki cihaz adını seçin.</span><span class="sxs-lookup"><span data-stu-id="5e910-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="5e910-117">**Cihazlar listesi** - Cihazlar listesinden cihazın adını seçin.</span><span class="sxs-lookup"><span data-stu-id="5e910-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="5e910-118">**Arama kutusu** - Açılan menüden Cihaz'ı seçin ve cihazın adını girin.</span><span class="sxs-lookup"><span data-stu-id="5e910-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="5e910-119">Ayrıca, dosya ve IP görünümleri üzerinden uyarı sayfasına da çıkabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5e910-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="5e910-120">Yanıt **eylemleri satırından** Etiketleri Yönet'i seçin.</span><span class="sxs-lookup"><span data-stu-id="5e910-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="5e910-121">Etiketleri bulmak veya oluşturmak için yazın.</span><span class="sxs-lookup"><span data-stu-id="5e910-121">Type to find or create tags.</span></span>

<span data-ttu-id="5e910-122">Etiketler cihaz görünümüne eklenir ve Cihazlar liste görünümünde yansıtılmaktadır.</span><span class="sxs-lookup"><span data-stu-id="5e910-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="5e910-123">Daha sonra ilgili cihaz listesini görmek için Etiketler filtresini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="5e910-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="5e910-124">Daha fazla bilgi için [bkz. Cihaz etiketlerini oluşturma ve yönetme.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="5e910-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>