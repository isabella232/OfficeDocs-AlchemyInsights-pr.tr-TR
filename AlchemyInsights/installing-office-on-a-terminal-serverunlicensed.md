---
title: Office 'i Terminal sunucusuna yükleme-lisanssız
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663137"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="ba542-102">Office 'i Terminal sunucusuna yükleme</span><span class="sxs-lookup"><span data-stu-id="ba542-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="ba542-103">Windows Server 'da kurumsal olarak Microsoft 365 uygulamalarını dağıtmak için, eski adıyla Terminal Hizmetleri adlı uzak Masaüstü Hizmetleri (RDS) kullanın:</span><span class="sxs-lookup"><span data-stu-id="ba542-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="ba542-104">Office 365 Kurumsal E3 veya Kurumsal E5 gibi kuruluş için Microsoft 365 uygulamalarını içeren bir Microsoft 365 aboneliğiniz olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="ba542-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="ba542-105">İş için Microsoft 365 uygulamaları ve Microsoft 365 Uygulamaları İş Ekstra planları için Microsoft 365 uygulamaları bulunmaz.</span><span class="sxs-lookup"><span data-stu-id="ba542-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="ba542-106">[Paylaşılan bilgisayar etkinleştirmesini](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)etkinleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="ba542-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="ba542-107">***Varsayılan yükleme ayarlarını kullanan***Microsoft 365 Yönetim merkezinden kuruluş için Microsoft 365 uygulamalarını yüklemek istiyorsanız, aşağıdaki adımları kullanın.</span><span class="sxs-lookup"><span data-stu-id="ba542-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="ba542-108">Paylaşılan bilgisayar etkinleştirme modu 'nda kuruluş için Microsoft 365 uygulamalarını yüklemek üzere [Microsoft destek ve Kurtarma Yardımcısı](https://aka.ms/SaRA_OfficeSCA_M365Portal) 'nı indirebilir ve çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ba542-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="ba542-109">Sahip olduğunuz Microsoft 365 aboneliğini denetleyin.</span><span class="sxs-lookup"><span data-stu-id="ba542-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="ba542-110">Nasıl yapıldığını öğrenin</span><span class="sxs-lookup"><span data-stu-id="ba542-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="ba542-111">Gerekirse, farklı bir Microsoft 365 aboneliğine geçin.</span><span class="sxs-lookup"><span data-stu-id="ba542-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="ba542-112">Nasıl yapıldığını öğrenin</span><span class="sxs-lookup"><span data-stu-id="ba542-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="ba542-113">Office, başka bir Microsoft 365 aboneliğini kullanarak RDS sunucusunda zaten yüklüyse kaldırın.</span><span class="sxs-lookup"><span data-stu-id="ba542-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="ba542-114">Örneğin, Denetim Masası 'Ndan \> bir program Kaldır 'a giderek.</span><span class="sxs-lookup"><span data-stu-id="ba542-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="ba542-115">Sorun yaşıyorsanız [Microsoft destek ve Kurtarma Yardımcısı 'nı](https://aka.ms/SARA-OfficeUninstall-Alchemy) kullanarak kaldırın.</span><span class="sxs-lookup"><span data-stu-id="ba542-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="ba542-116">RDS sunucusunda, Yönetici hesabınızla Microsoft 365 Yönetim Merkezi 'nde oturum açın ve [Kurumsal Için microsoft 365 uygulamalarını yükleyin](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="ba542-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="ba542-117">Office yüklendikten sonra, hiçbir Office uygulamasında ***açmayın veya oturum açmayın*** .</span><span class="sxs-lookup"><span data-stu-id="ba542-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="ba542-118">RDS sunucusunda, aşağıdaki adımları izleyerek kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirmesini etkinleştirin:</span><span class="sxs-lookup"><span data-stu-id="ba542-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="ba542-119">Ekranınızın sol alt köşesindeki Windows düğmesine sağ tıklayın ve sonra da Run 'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="ba542-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="ba542-120">Aç kutusuna **Regedit**yazın ve Tamam 'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="ba542-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="ba542-121">Kayıt Defteri Düzenleyicisi 'nin cihazınızda değişiklik yapmasına izin vermeniz istendiğinde Evet 'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="ba542-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="ba542-122">Kayıt Defteri Düzenleyicisi 'nde, HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\clicktorun\configurationaltında 1 ayarına sahip **Sharedcomputerlicensing** dize değerini ekleyin.</span><span class="sxs-lookup"><span data-stu-id="ba542-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="ba542-123">RDS sunucusunda ***Son Kullanıcı olarak oturum açın*** ve [paylaşılan bilgisayar etkinleştirmenin Kurumsal Microsoft 365 uygulamaları için etkinleştirildiğini doğrulayın](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="ba542-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="ba542-124">Önkoşullar hakkında daha fazla bilgi için, Office dağıtım Aracı kullanılarak özelleştirilmiş yüklemelerde [Microsoft 365 uygulamalarını dağıtma](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="ba542-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="ba542-125">Paylaşılan bilgisayar etkinleştirme ile ilgili hataları düzeltmek için, lütfen [Enterprise Için Microsoft 365 uygulamalarında paylaşılan bilgisayar etkinleştirme sorunlarını giderme](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="ba542-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  