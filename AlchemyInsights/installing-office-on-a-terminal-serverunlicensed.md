---
title: Bir Terminal sunucusunda - lisanssız Office yükleme
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6fc4bd5f6971ca833084a6a8ad6c25b3fdafb8dc
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35381749"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="f6973-102">Office bir Terminal sunucusuna program yükleme</span><span class="sxs-lookup"><span data-stu-id="f6973-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="f6973-103">Uzak Masaüstü Hizmetleri (RDS) kullanan Windows Server Office 365 ProPlus dağıtmak için önceden Terminal Hizmetleri olarak adlandırılan:</span><span class="sxs-lookup"><span data-stu-id="f6973-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="f6973-104">Office 365 ProPlus, Office 365 Kurumsal E3 veya Kurumsal E5 gibi içeren bir Office 365 planınız olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="f6973-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="f6973-105">Office 365 iş ve Office 365 iş Premium planları Office 365 ProPlus dahil etmeyin.</span><span class="sxs-lookup"><span data-stu-id="f6973-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="f6973-106">[Paylaşılan bilgisayar](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)etkinleştirmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="f6973-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="f6973-107">Office 365 ProPlus RDS üzerinde Office 365 portalından yüklemek istiyorsanız \*\* *varsayılan yükleme ayarlarını kullanan* \*\*, şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="f6973-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span>
  
1. <span data-ttu-id="f6973-108">Elinizde hangi Office 365 planını denetleyin.</span><span class="sxs-lookup"><span data-stu-id="f6973-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="f6973-109">Öğrenin nasıl</span><span class="sxs-lookup"><span data-stu-id="f6973-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="f6973-110">Gerekirse, başka bir Office 365 anahtarı düşünüyorsanız.</span><span class="sxs-lookup"><span data-stu-id="f6973-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="f6973-111">Öğrenin nasıl</span><span class="sxs-lookup"><span data-stu-id="f6973-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="f6973-112">Diğer Office 365 planları kullanarak RDS Sunucu üzerinde Office yüklüyse, kaldırın.</span><span class="sxs-lookup"><span data-stu-id="f6973-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="f6973-113">Örneğin, Denetim Masası'na giderek tarafından \> program Kaldır.</span><span class="sxs-lookup"><span data-stu-id="f6973-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="f6973-114">Sorunlar çalıştırıyorsanız, [Microsoft destek ve kurtarma Yardımcısı'nı](https://aka.ms/SARA-OfficeUninstall-Alchemy) kullanarak kaldırın.</span><span class="sxs-lookup"><span data-stu-id="f6973-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="f6973-115">RDS Sunucu üzerinde yönetici hesabı ve [Office 365 ProPlus yüklemek](https://portal.office.com/OLS/MySoftware.aspx)Office 365 portalına oturum açın.</span><span class="sxs-lookup"><span data-stu-id="f6973-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="f6973-116">Office yüklendikten sonra \*\* *açmayın veya oturum* \*\* tüm Office uygulamaları için.</span><span class="sxs-lookup"><span data-stu-id="f6973-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span>

6. <span data-ttu-id="f6973-117">RDS Sunucu üzerinde aaıdaki adımları izleyerek kayıt defterini düzenleyerek paylaşılan bilgisayar etkinleştirme etkinleştir:</span><span class="sxs-lookup"><span data-stu-id="f6973-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="f6973-118">Ekranın sol alt köşesinde Windows düğmesini sağ tıklatın ve Çalıştır'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="f6973-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="f6973-119">Aç kutusuna **regedit**yazın ve Tamam'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="f6973-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="f6973-120">Evet, aygıtınız için değişiklik yapmak için Kayıt Defteri Düzenleyicisi'ni izin vermek isteyip istemediğiniz sorulduğunda seçin.</span><span class="sxs-lookup"><span data-stu-id="f6973-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="f6973-121">Kayıt Defteri Düzenleyicisi'nde, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration altında 1 ayarı ile **SharedComputerLicensing** bir dize değeri ekleyin.</span><span class="sxs-lookup"><span data-stu-id="f6973-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="f6973-122">RDS Sunucu üzerindeki \*\* *bir son kullanıcı oturum aç* \*\* ve [paylaşılan bilgisayar etkinleştirme Office 365 ProPlus için etkinleştirilmiş olduğunu doğrulayın](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="f6973-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="f6973-123">Önkoşullar, kurulum yönergelerini ve Office Dağıtım Aracı'nı kullanarak özelleştirilmiş yüklemeleri Kılavuzu hakkında daha fazla ayrıntı için lütfen [Dağıtmak Office 365 Uzak Masaüstü Hizmetleri kullanarak ProPlus](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)bakın.</span><span class="sxs-lookup"><span data-stu-id="f6973-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="f6973-124">Paylaşılan bilgisayar etkinleştirme için ilgili hataları gidermek için [Office 365 ProPlus için paylaşılan bilgisayar etkinleştirme ile ilgili sorunları giderme](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="f6973-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  