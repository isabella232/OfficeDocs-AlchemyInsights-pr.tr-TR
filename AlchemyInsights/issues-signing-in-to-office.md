---
title: Microsoft 365 uygulamalarında oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579921"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="ece3d-102">Microsoft 365 uygulamalarında boş oturum açma ekranı</span><span class="sxs-lookup"><span data-stu-id="ece3d-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="ece3d-103">Bu sorunu gidermek için aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="ece3d-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="ece3d-104">[Windows](https://support.microsoft.com/help/4027667/windows-10-update) ve [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)için en son güncelleştirmeleri yükleyin.</span><span class="sxs-lookup"><span data-stu-id="ece3d-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="ece3d-105">Internet Explorer seçeneklerini sıfırla: **Araçlar**  >  **Internet Seçenekleri**  >  **Gelişmiş**Sıfırlama Internet  >  **Explorer Ayarlarını** (özel ayarları kaybedeceğinizi unutmayın) gidin ve ardından Office'te yeniden oturum açmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="ece3d-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="ece3d-106">Windows Defender Application Guard (WDAG) veya benzer bir güvenlik duvarı veya anti-virüs programı devre dışı:</span><span class="sxs-lookup"><span data-stu-id="ece3d-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="ece3d-107">Denetim Masası'nda **Programlar'a**gidin ve ardından **Windows özelliklerini açıp kapatmayı**seçin.</span><span class="sxs-lookup"><span data-stu-id="ece3d-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="ece3d-108">Windows Defender Application Guard etkinse, devre dışı bırakmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="ece3d-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="ece3d-109">**Not:** Bilgisayarı yeniden başlatmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="ece3d-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="ece3d-110">Microsoft.AAD.BrokerPlugin [AAD WAM eklentisinin](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) herhangi bir uygulama veya güvenlik duvarı/virüsten koruma programı tarafından engellenmediğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="ece3d-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="ece3d-111">Windows Kimlik Bilgileri Yöneticisi'ni kullanarak [Office kimlik bilgilerini temizleyin.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)</span><span class="sxs-lookup"><span data-stu-id="ece3d-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="ece3d-112">**Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değiştirildi.</span><span class="sxs-lookup"><span data-stu-id="ece3d-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="ece3d-113">(Ör. \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="ece3d-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="ece3d-114">Daha fazla bilgi için bkz: [Windows 10'da Office 2016'da 16.0.7967'yi oluştur'a güncellemeden sonra oturum açma](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)bağlantısı sorunları.</span><span class="sxs-lookup"><span data-stu-id="ece3d-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>