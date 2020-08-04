---
title: Intune aygıtlarını uzaktan yönetmek için TeamViewer'ı kullanma
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555753"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="f06aa-102">Intune aygıtlarını uzaktan yönetmek için TeamViewer'ı kullanma</span><span class="sxs-lookup"><span data-stu-id="f06aa-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="f06aa-103">Intune tarafından yönetilen aygıtlar [TeamViewer](https://www.teamviewer.com/)kullanılarak uzaktan yönetilebilir.</span><span class="sxs-lookup"><span data-stu-id="f06aa-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="f06aa-104">TeamViewer'ı kullanarak Intune'u yönetmek için şu adımları kullanın:</span><span class="sxs-lookup"><span data-stu-id="f06aa-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="f06aa-105">Intune'da TeamViewer Bağlayıcısı'nı kurmak için TeamViewer'dan kimlik bilgileri alarak başlayın.</span><span class="sxs-lookup"><span data-stu-id="f06aa-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="f06aa-106">Bu, yöneticinin Intune ve TeamViewer hizmeti arasındaki bağlantıyı kurmak için bir kerelik işlem olan Aygıtlar altında TeamViewer Bağlayıcı Ara Birimi'ne kimlik bilgilerini girmesini sağlar.</span><span class="sxs-lookup"><span data-stu-id="f06aa-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="f06aa-107">**Bölüm 1: Oturumu uzak bir aygıtla başlatma**</span><span class="sxs-lookup"><span data-stu-id="f06aa-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="f06aa-108">**Tüm aygıtların**altında, uzaktan oturum başlatmak istediğiniz aygıtı seçin.</span><span class="sxs-lookup"><span data-stu-id="f06aa-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="f06aa-109">Kaynak: **... Daha fazla**, **Yeni uzaktan yardım oturumu**seçin.</span><span class="sxs-lookup"><span data-stu-id="f06aa-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="f06aa-110">Uzak bir oturum oluşturmak istediğinizi kabul etmek için **Evet'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="f06aa-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="f06aa-111">"Yeni bir uzaktan oturum başlatma" isteği TeamViewer hizmeti tarafından onaylandıktan sonra, aygıt için Genel Bakış (veya Temel Bilgiler) bölmesinin ayrıntıları altında **uzaktan yardımı başlatma** seçeneğini görürsünüz.</span><span class="sxs-lookup"><span data-stu-id="f06aa-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="f06aa-112">Bölmeyi genişletmek ve Uzaktan Yardım durumunu göstermek için **Daha Fazla yı** seçin.</span><span class="sxs-lookup"><span data-stu-id="f06aa-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="f06aa-113">Oturumu yönetici tarafında başlatmak için **uzak oturumu başlat'ı** seçin.</span><span class="sxs-lookup"><span data-stu-id="f06aa-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="f06aa-114">TeamViewer ikilisini (Windows) indirmeyi seçin ve **Çalıştır'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="f06aa-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="f06aa-115">**Not** TeamViewer web sitesine açılan herhangi bir web tarayıcısayfasını yok sayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f06aa-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="f06aa-116">TeamViewer uygulamasının aygıtta değişiklik yapma isteğini kabul edin (yalnızca Windows).</span><span class="sxs-lookup"><span data-stu-id="f06aa-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="f06aa-117">TeamViewer uygulaması başlatılır ve uzak aygıtla bağlantının kimliğini doğrulamak için oturum kodunu içerir.</span><span class="sxs-lookup"><span data-stu-id="f06aa-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="f06aa-118">**Bölüm 2: Uzak bir oturum için hedeflenen aygıtta**</span><span class="sxs-lookup"><span data-stu-id="f06aa-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="f06aa-119">Intune şirket portalını açın.</span><span class="sxs-lookup"><span data-stu-id="f06aa-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="f06aa-120">Bildirim bayrağına bakın: "BT yöneticiniz uzaktan yardım oturumu için bu aygıtın denetimini istiyor" ve bildirimi seçin.</span><span class="sxs-lookup"><span data-stu-id="f06aa-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="f06aa-121">TeamViewer uygulamasını indirmeyi seçin veya TeamViewer uygulamasının uygulama mağazasından indirilmeyi kabul edin ve **Çalıştır'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="f06aa-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="f06aa-122">**Not** TeamViewer web sitesine açılan herhangi bir web tarayıcısayfasını yok sayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f06aa-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="f06aa-123">TeamViewer uygulamasının aygıtta değişiklik yapma isteğini kabul edin (yalnızca Windows).</span><span class="sxs-lookup"><span data-stu-id="f06aa-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="f06aa-124">TeamViewer uygulaması başlatılır ve uzak aygıtla bağlantının kimliğini doğrulamak için oturum kodunu içerir.</span><span class="sxs-lookup"><span data-stu-id="f06aa-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="f06aa-125">Açılır pencere, oturumun başlamasına izin vermek isteyip istemediğinizi sorar.</span><span class="sxs-lookup"><span data-stu-id="f06aa-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="f06aa-126">**Not** TeamViewer hizmeti tarafından oluşturulan oturum kodları yalnızca tek seferlik kullanımdır.</span><span class="sxs-lookup"><span data-stu-id="f06aa-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="f06aa-127">Bağlantıyı kaybederseniz, şunları</span><span class="sxs-lookup"><span data-stu-id="f06aa-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="f06aa-128">TeamViewer uygulamasıörneğini uzak aygıtta ve yönetici iş istasyonunda kapatın.</span><span class="sxs-lookup"><span data-stu-id="f06aa-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="f06aa-129">Uzak aygıttaki şirket portalını kapatın.</span><span class="sxs-lookup"><span data-stu-id="f06aa-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="f06aa-130">Yönetici portalından yeni bir "Yeni uzaktan Yardım oturumu" başlatın.</span><span class="sxs-lookup"><span data-stu-id="f06aa-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="f06aa-131">Yeni bildirimi almak için uzak aygıttaki şirket portalını yeniden açın.</span><span class="sxs-lookup"><span data-stu-id="f06aa-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="f06aa-132">TeamViewer uygulamasını daha önce olduğu gibi hem uzak aygıtta hem de yönetici iş istasyonunda indirin ve açın.</span><span class="sxs-lookup"><span data-stu-id="f06aa-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>