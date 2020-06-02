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
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508648"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="52eff-102">Terminal Sunucusuna Office Yükleme</span><span class="sxs-lookup"><span data-stu-id="52eff-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="52eff-103">Eskiden Terminal Hizmetleri olarak adlandırılan Uzak Masaüstü Hizmetleri 'ni (RDS) kullanarak Windows Server'da kurumsal olarak Microsoft 365 Uygulamaları dağıtmak için:</span><span class="sxs-lookup"><span data-stu-id="52eff-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="52eff-104">Office 365 Enterprise E3 veya Enterprise E5 gibi kurumsal microsoft 365 Uygulamalarını içeren bir Microsoft 365 aboneliğiniz olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="52eff-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="52eff-105">Microsoft 365 İş Uygulamaları ve Microsoft 365 İş Premium planları için Uygulamalar, kurumsal için Microsoft 365 Apps'ı içermez.</span><span class="sxs-lookup"><span data-stu-id="52eff-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="52eff-106">Paylaşılan bilgisayar [etkinleştirmesini](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)etkinleştirmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="52eff-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="52eff-107">***Varsayılan yükleme ayarlarını kullanan***Microsoft 365 yönetici merkezinden RDS'de kurumsal olarak Microsoft 365 Uygulamaları yüklemek istiyorsanız, aşağıdaki adımları kullanın.</span><span class="sxs-lookup"><span data-stu-id="52eff-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="52eff-108">Microsoft 365 Apps for enterprise'ı paylaşılan bilgisayar etkinleştirme modunda yüklemek için [Microsoft Destek ve Kurtarma Yardımcısı'nı](https://aka.ms/SaRA_OfficeSCA_M365Portal) da indirip çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="52eff-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="52eff-109">Hangi Microsoft 365 aboneliğine sahip olduğunuzu kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="52eff-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="52eff-110">Nasıl yapılacağını öğrenin</span><span class="sxs-lookup"><span data-stu-id="52eff-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="52eff-111">Gerekirse, farklı bir Microsoft 365 aboneliğine geçin.</span><span class="sxs-lookup"><span data-stu-id="52eff-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="52eff-112">Nasıl yapılacağını öğrenin</span><span class="sxs-lookup"><span data-stu-id="52eff-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="52eff-113">Office, rds sunucusunda başka microsoft 365 abonelikleri kullanıyorsa, kaldırın.</span><span class="sxs-lookup"><span data-stu-id="52eff-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="52eff-114">Örneğin, Denetim Masası'na giderek \> bir programı kaldırın.</span><span class="sxs-lookup"><span data-stu-id="52eff-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="52eff-115">Sorunlarla karşınıza yüzde lerak [Microsoft Destek ve Kurtarma Yardımcısı'nı](https://aka.ms/SARA-OfficeUninstall-Alchemy) kullanarak kaldırın.</span><span class="sxs-lookup"><span data-stu-id="52eff-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="52eff-116">RDS sunucusunda, yönetici hesabınızla Microsoft 365 yönetici merkezinde oturum açın ve [kurumsal için Microsoft 365 Uygulamaları'nı yükleyin.](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="52eff-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="52eff-117">Office yüklendikten sonra, hiçbir Office uygulamasını ***açmayın veya oturum açmayın.***</span><span class="sxs-lookup"><span data-stu-id="52eff-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="52eff-118">RDS sunucusunda, aşağıdaki adımları izleyerek kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirmesini etkinleştirin:</span><span class="sxs-lookup"><span data-stu-id="52eff-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="52eff-119">Ekranınızın sol alt köşesindeki Windows düğmesine sağ tıklayın ve Çalıştır'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="52eff-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="52eff-120">Aç kutusunda **regedit**yazın ve ardından Tamam'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="52eff-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="52eff-121">Kayıt Defteri Düzenleyicisi'nin cihazınızda değişiklik yapmasına izin vermek istendiğinde Evet'i seçin.</span><span class="sxs-lookup"><span data-stu-id="52eff-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="52eff-122">Kayıt Defteri Düzenleyicisi'nde, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration altında 1 ayarı olan **Paylaşılan Bilgisayar Lisanslama** dize değeri ekleyin.</span><span class="sxs-lookup"><span data-stu-id="52eff-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="52eff-123">RDS sunucusunda, ***son kullanıcı olarak oturum açın*** ve microsoft [365 Kurumsal Uygulamalar için paylaşılan bilgisayar etkinleştirme etkinleştirme etkin olduğunu doğrulayın.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)</span><span class="sxs-lookup"><span data-stu-id="52eff-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="52eff-124">Office Dağıtım Aracı'nı kullanarak özelleştirilmiş yüklemelerle ilgili ön koşullar, kurulum talimatları ve kılavuzlar hakkında daha fazla bilgi için lütfen [Uzak Masaüstü Hizmetlerini kullanarak Microsoft 365 Uygulamalarını kurumsal olarak dağıt'a](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)bakın.</span><span class="sxs-lookup"><span data-stu-id="52eff-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="52eff-125">Paylaşılan bilgisayar etkinleştirmesiyle ilgili hataları gidermek için lütfen [Microsoft 365 Apps for enterprise için paylaşılan bilgisayar etkinleştirme sorunları bölümüne](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)bakın.</span><span class="sxs-lookup"><span data-stu-id="52eff-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  