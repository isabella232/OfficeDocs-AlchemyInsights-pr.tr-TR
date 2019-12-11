---
title: RDS, Terminal Server veya VDI'de paylaşılan kullanım için Office 365 ProPlus'ı dağıtma
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959479"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="14a4b-102">RDS, Terminal Server veya VDI'de paylaşılan kullanım için Office 365 ProPlus'ı dağıtma</span><span class="sxs-lookup"><span data-stu-id="14a4b-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="14a4b-103">Office 365 ProPlus'ı, eskiden Terminal Hizmetleri olarak adlandırılan Uzak Masaüstü Hizmetlerini (RDS) kullanarak dağıtmak için:</span><span class="sxs-lookup"><span data-stu-id="14a4b-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="14a4b-104">Bir Microsoft 365 İşletmeler İçin planınız veya Office 365 ProPlus içeren Office 365 Planı(Office 365 Enterprise E3 veya Enterprise E5 gibi) olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="14a4b-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="14a4b-105">Office 365 Business ve Office 365 Business Premium planları Office 365 ProPlus'ı içermez.</span><span class="sxs-lookup"><span data-stu-id="14a4b-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="14a4b-106">[Paylaşılan bilgisayar etkinleştirmesini](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)etkinleştirmelisiniz.</span><span class="sxs-lookup"><span data-stu-id="14a4b-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="14a4b-107">Office 365 ProPlus'ı paylaşılan bilgisayar etkinleştirme modunda yüklemek için [Microsoft Destek ve Kurtarma Yardımcısı'nı](https://aka.ms/SaRA_OfficeSCA_M365Portal) indirip çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="14a4b-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="14a4b-108">Office Dağıtım Aracı'nı kullanarak ön koşullar, kurulum talimatları ve özelleştirilmiş yüklemeler hakkında daha fazla bilgi için, [Uzak Masaüstü Hizmetlerini kullanarak Office 365 ProPlus'ı dağıt'a](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)bakın.</span><span class="sxs-lookup"><span data-stu-id="14a4b-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="14a4b-109">Paylaşılan bilgisayar etkinleştirmeyle ilgili hataları düzeltmek için:</span><span class="sxs-lookup"><span data-stu-id="14a4b-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="14a4b-110">[Office 365 ProPlus için paylaşılan bilgisayar etkinleştirme siyle ilgili Sorun Giderme sorunlarına](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)bakın.</span><span class="sxs-lookup"><span data-stu-id="14a4b-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="14a4b-111">Bkz. [Office 365 ProPlus etkinleştirme durumunu sıfırla.](https://go.microsoft.com/fwlink/?linkid=2109218)</span><span class="sxs-lookup"><span data-stu-id="14a4b-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="14a4b-112">***Varsayılan yükleme ayarlarını kullanan***Microsoft 365 yönetici merkezinden RDS'ye Office 365 ProPlus'ı yüklemek istiyorsanız, aşağıdaki adımları kullanın:</span><span class="sxs-lookup"><span data-stu-id="14a4b-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="14a4b-113">Hangi Office 365 planınız olup deiyi kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="14a4b-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="14a4b-114">[Nasıl yapıldığını öğrenin](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="14a4b-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="14a4b-115">Gerekirse, farklı bir Office 365 planına geçin.</span><span class="sxs-lookup"><span data-stu-id="14a4b-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="14a4b-116">[Nasıl yapıldığını öğrenin](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="14a4b-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="14a4b-117">Office, diğer Office 365 planlarını kullanarak RDS sunucusuna zaten yüklüyse, kaldırın.</span><span class="sxs-lookup"><span data-stu-id="14a4b-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="14a4b-118">Örneğin, **Denetim Masası'na** > giderek**bir programı kaldırın.**</span><span class="sxs-lookup"><span data-stu-id="14a4b-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="14a4b-119">Sorunlarla karşınıza yüzde lerak [Microsoft Destek ve Kurtarma Yardımcısı'nı](https://aka.ms/SARA-OfficeUninstall-Alchemy) kullanarak kaldırın.</span><span class="sxs-lookup"><span data-stu-id="14a4b-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="14a4b-120">RDS sunucusunda, yönetici hesabınızla Microsoft 365 yönetici merkezinde oturum açın ve [Office 365 ProPlus'ı yükleyin.](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="14a4b-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="14a4b-121">Office yüklendikten sonra, hiçbir Office uygulamasını ***açmayın veya oturum açmayın.***</span><span class="sxs-lookup"><span data-stu-id="14a4b-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="14a4b-122">RDS sunucusunda, aşağıdaki adımları izleyerek kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirmesini etkinleştirin:</span><span class="sxs-lookup"><span data-stu-id="14a4b-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="14a4b-123">Ekranınızın sol alt köşesindeki Windows düğmesine sağ tıklayın ve **Çalıştır'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="14a4b-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="14a4b-124">Açık kutusunda **regedit**yazın ve ardından **Tamam'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="14a4b-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="14a4b-125">Kayıt Defteri Düzenleyicisi'nin cihazınızda değişiklik yapmasına izin vermek istendiğinde **Evet'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="14a4b-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="14a4b-126">Kayıt Defteri Düzenleyicisi'nde, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration altında 1 ayarı olan **Paylaşılan Bilgisayar Lisanslama** dize değeri ekleyin.</span><span class="sxs-lookup"><span data-stu-id="14a4b-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="14a4b-127">RDS sunucusunda, ***son kullanıcı olarak oturum açın*** ve Paylaşılan bilgisayar [etkinleştirme Office 365 ProPlus için etkinleştirildiğinden doğrulayın.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)</span><span class="sxs-lookup"><span data-stu-id="14a4b-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

