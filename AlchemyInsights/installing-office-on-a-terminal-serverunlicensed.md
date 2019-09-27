---
title: Terminal Sunucusuna ofis yükleme - Lisanssız
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205429"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="b569e-102">Terminal Sunucusuna Office Yükleme</span><span class="sxs-lookup"><span data-stu-id="b569e-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="b569e-103">Office 365 ProPlus'ı, eskiden Terminal Hizmetleri olarak adlandırılan Uzak Masaüstü Hizmetlerini (RDS) kullanarak bir Windows Server'da dağıtmak için:</span><span class="sxs-lookup"><span data-stu-id="b569e-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="b569e-104">Office 365 ProPlus'ı içeren Office 365 planınız olmalıdır(Office 365 Enterprise E3 veya Enterprise E5).</span><span class="sxs-lookup"><span data-stu-id="b569e-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="b569e-105">Office 365 Business ve Office 365 Business Premium planları Office 365 ProPlus'ı içermez.</span><span class="sxs-lookup"><span data-stu-id="b569e-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="b569e-106">Paylaşılan bilgisayar [etkinleştirmesini](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)etkinleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="b569e-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="b569e-107">***Varsayılan yükleme ayarlarını kullanan***Microsoft 365 yönetici merkezinden RDS'ye Office 365 ProPlus'ı yüklemek istiyorsanız, aşağıdaki adımları kullanın.</span><span class="sxs-lookup"><span data-stu-id="b569e-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="b569e-108">Office 365 ProPlus'ı paylaşılan bilgisayar etkinleştirme modunda yüklemek için [Microsoft Destek ve Kurtarma Yardımcısı'nı](https://aka.ms/SaRA_OfficeSCA_M365Portal) indirip çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b569e-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="b569e-109">Hangi Office 365 planınız olup deiyi kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="b569e-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="b569e-110">Nasıl yapılacağını öğrenin</span><span class="sxs-lookup"><span data-stu-id="b569e-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="b569e-111">Gerekirse, farklı bir Office 365 planına geçin.</span><span class="sxs-lookup"><span data-stu-id="b569e-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="b569e-112">Nasıl yapılacağını öğrenin</span><span class="sxs-lookup"><span data-stu-id="b569e-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="b569e-113">Office, diğer Office 365 planlarını kullanarak RDS sunucusuna zaten yüklüyse, kaldırın.</span><span class="sxs-lookup"><span data-stu-id="b569e-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="b569e-114">Örneğin, Denetim Masası'na \> giderek bir programı kaldırın.</span><span class="sxs-lookup"><span data-stu-id="b569e-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="b569e-115">Sorunlarla karşınıza yüzde lerak [Microsoft Destek ve Kurtarma Yardımcısı'nı](https://aka.ms/SARA-OfficeUninstall-Alchemy) kullanarak kaldırın.</span><span class="sxs-lookup"><span data-stu-id="b569e-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="b569e-116">RDS sunucusunda, yönetici hesabınızla Microsoft 365 yönetici merkezinde oturum açın ve [Office 365 ProPlus'ı yükleyin.](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="b569e-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="b569e-117">Office yüklendikten sonra, hiçbir Office uygulamasını ***açmayın veya oturum açmayın.***</span><span class="sxs-lookup"><span data-stu-id="b569e-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="b569e-118">RDS sunucusunda, aşağıdaki adımları izleyerek kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirmesini etkinleştirin:</span><span class="sxs-lookup"><span data-stu-id="b569e-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="b569e-119">Ekranınızın sol alt köşesindeki Windows düğmesine sağ tıklayın ve Çalıştır'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b569e-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="b569e-120">Aç kutusunda **regedit**yazın ve ardından Tamam'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="b569e-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="b569e-121">Kayıt Defteri Düzenleyicisi'nin cihazınızda değişiklik yapmasına izin vermek istendiğinde Evet'i seçin.</span><span class="sxs-lookup"><span data-stu-id="b569e-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="b569e-122">Kayıt Defteri Düzenleyicisi'nde, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration altında 1 ayarı ile **Paylaşılan Bilgisayar Lisanslama** dize değeri ekleyin.</span><span class="sxs-lookup"><span data-stu-id="b569e-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="b569e-123">RDS sunucusunda, ***son kullanıcı olarak oturum açın*** ve Paylaşılan bilgisayar [etkinleştirme Office 365 ProPlus için etkinleştirildiğinden doğrulayın.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)</span><span class="sxs-lookup"><span data-stu-id="b569e-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="b569e-124">Office Dağıtım Aracı'nı kullanarak ön koşullar, kurulum talimatları ve özelleştirilmiş yüklemelerle ilgili kılavuzlar hakkında daha fazla bilgi için lütfen [Uzak Masaüstü Hizmetlerini kullanarak Office 365 ProPlus'ı dağıt'a](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)bakın.</span><span class="sxs-lookup"><span data-stu-id="b569e-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="b569e-125">Paylaşılan bilgisayar etkinleştirmesiyle ilgili hataları gidermek [için, Office 365 ProPlus için paylaşılan bilgisayar etkinleştirme sorunları bölümüne](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)bakın.</span><span class="sxs-lookup"><span data-stu-id="b569e-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  