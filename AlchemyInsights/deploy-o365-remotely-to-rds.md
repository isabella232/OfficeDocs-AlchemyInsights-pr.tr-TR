---
title: RDS, Terminal Server veya VDI'de paylaşılan kullanım için kuruluş için Microsoft 365 Uygulamalarını dağıtma
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200693"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="68c0f-102">RDS, Terminal Server veya VDI'de paylaşılan kullanım için kuruluş için Microsoft 365 Uygulamalarını dağıtma</span><span class="sxs-lookup"><span data-stu-id="68c0f-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="68c0f-103">Eski adı Terminal Hizmetleri olan Uzak Masaüstü Hizmetleri'ni (RDS) kullanarak kuruluşa Microsoft 365 Uygulamalarını dağıtmak için:</span><span class="sxs-lookup"><span data-stu-id="68c0f-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="68c0f-104">Microsoft 365 İş planınız veya Office 365 Kurumsal E3 veya Kurumsal E5 gibi kurumsal Microsoft 365 Uygulamaları içeren bir Office 365 planınız olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="68c0f-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="68c0f-105">İşletmeler için Microsoft 365 Uygulamaları ve Microsoft 365 İş Standart planları, kuruluş için Microsoft 365 Uygulamalarını içermez.</span><span class="sxs-lookup"><span data-stu-id="68c0f-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="68c0f-106">Paylaşılan bilgisayar [etkinleştirmeyi etkinleştirmeniz gerekir.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="68c0f-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="68c0f-107">Ayrıca, paylaşılan bilgisayar etkinleştirme modunda [kuruluş için Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) 365 Uygulamalarını yüklemek için Microsoft Destek ve Kurtarma Yardımcısı'ı indirip çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="68c0f-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="68c0f-108">Office Dağıtım Aracı'nı kullanarak özelleştirilmiş yüklemeler hakkında önkoşullar, kurulum yönergeleri ve yönergeler hakkında daha fazla bilgi için, Uzak Masaüstü Hizmetleri'nı kullanarak kuruluş için [Microsoft 365 Uygulamalarını Dağıtma'ya bakın.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)</span><span class="sxs-lookup"><span data-stu-id="68c0f-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="68c0f-109">Paylaşılan bilgisayar etkinleştirmeyle ilgili hataları düzeltmek için:</span><span class="sxs-lookup"><span data-stu-id="68c0f-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="68c0f-110">Kurumsal [Microsoft 365 Uygulamaları için paylaşılan bilgisayar etkinleştirme sorunlarını giderme makalesine bakın.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="68c0f-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="68c0f-111">Bkz. [Kuruluşlar için Microsoft 365 Uygulamaları etkinleştirme durumunu sıfırlama](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="68c0f-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="68c0f-112">Varsayılan yükleme ayarlarını kullanan Microsoft 365 yönetim merkezinden RDS'ye kuruluş için Microsoft 365 Uygulamalarını yüklemek için ***aşağıdaki*** adımları kullanın:</span><span class="sxs-lookup"><span data-stu-id="68c0f-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="68c0f-113">Hangi aboneliğe sahip olduğunu kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="68c0f-113">Check what subscription you have.</span></span> <span data-ttu-id="68c0f-114">[Nasıl yapıldığını öğrenin](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="68c0f-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="68c0f-115">Gerekirse farklı bir aboneliğe geçin.</span><span class="sxs-lookup"><span data-stu-id="68c0f-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="68c0f-116">[Nasıl yapıldığını öğrenin](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="68c0f-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="68c0f-117">Office diğer Microsoft aboneliklerini kullanarak RDS sunucusuna zaten yüklenmişse kaldırın.</span><span class="sxs-lookup"><span data-stu-id="68c0f-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="68c0f-118">Örneğin Denetim Masası'nı **kullanarak**  >  **programı kaldırın.**</span><span class="sxs-lookup"><span data-stu-id="68c0f-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="68c0f-119">Microsoft Destek [ve Kurtarma Yardımcısı'nın](https://aka.ms/SARA-OfficeUninstall-Alchemy) kullanımıyla ilgili sorunlar ile ilgili sorunları kaldırın.</span><span class="sxs-lookup"><span data-stu-id="68c0f-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="68c0f-120">RDS sunucusunda, yönetici hesabınızla Microsoft 365 yönetim merkezinde oturum açın ve kuruluş için [Microsoft 365 Uygulamalarını yükleyin.](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="68c0f-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="68c0f-121">Office yüklendikten sonra hiçbir Office ***uygulaması açmayın veya*** oturum açmayın.</span><span class="sxs-lookup"><span data-stu-id="68c0f-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="68c0f-122">RDS sunucusunda, aşağıdaki adımları kullanarak kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirmesini etkinleştirin:</span><span class="sxs-lookup"><span data-stu-id="68c0f-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="68c0f-123">Ekranın sol alt köşesindeki Windows düğmesine sağ tıklayın ve Çalıştır'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="68c0f-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="68c0f-124">Aç kutusuna, **regedit** yazın ve sonra da **Tamam**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="68c0f-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="68c0f-125">Kayıt **Defteri** Düzenleyicisi'nin aygıtınızda değişiklik yapmasına izin vermek istendiğinde Evet'i seçin.</span><span class="sxs-lookup"><span data-stu-id="68c0f-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="68c0f-126">Kayıt Defteri Düzenleyicisi'nde, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration altında 1 ayarıyla **SharedComputerLicensing'in** dize değerini ekleyin.</span><span class="sxs-lookup"><span data-stu-id="68c0f-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="68c0f-127">RDS sunucusunda ***son*** kullanıcı olarak oturum açma ve kuruluş için Microsoft 365 Uygulamaları için paylaşılan bilgisayar etkinleştirmenin [etkinleştirildiğinden emin olun.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)</span><span class="sxs-lookup"><span data-stu-id="68c0f-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>
