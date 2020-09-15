---
title: Microsoft 365 uygulamalarında oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695307"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="83934-102">Microsoft 365 uygulamalarında boş oturum açma ekranı</span><span class="sxs-lookup"><span data-stu-id="83934-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="83934-103">Bu sorunu çözmek için aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="83934-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="83934-104">En son [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ve [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)güncelleştirmelerini yükleyin.</span><span class="sxs-lookup"><span data-stu-id="83934-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="83934-105">Internet Explorer seçeneklerini sıfırlayın: araçlara gidin **Tools**  >  **İnternet seçenekleri**  >  **Gelişmiş**  >  **Internet Explorer ayarlarını sıfırlayın** (özel ayarları kaybedeceğinizi unutmayın) ve ardından Office 'te yeniden oturum açmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="83934-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="83934-106">Windows Defender Application Guard (WDAG) veya benzer bir güvenlik duvarını veya antivirüs programını devre dışı bırakın:</span><span class="sxs-lookup"><span data-stu-id="83934-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="83934-107">Denetim Masası 'nda, **Programlar**'a gidin ve **Windows özelliklerini aç veya kapat**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="83934-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="83934-108">Windows Defender Application Guard etkinse, devre dışı bırakmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="83934-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="83934-109">**Not:** Bilgisayarı yeniden başlatmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="83934-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="83934-110">Microsoft. AAD. BrokerPlugin [AAD WAM eklentisinin](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) herhangi bir uygulama veya güvenlik duvarı/virüs önleme programı tarafından engellenmediğinden emin olun.</span><span class="sxs-lookup"><span data-stu-id="83934-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="83934-111">Windows kimlik bilgileri Yöneticisi 'Ni kullanarak [Office kimlik bilgilerini temizleyin](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .</span><span class="sxs-lookup"><span data-stu-id="83934-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="83934-112">**Not:** Office 2016 için kayıt defteri yolları 16,0 olarak değiştirilmiştir.</span><span class="sxs-lookup"><span data-stu-id="83934-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="83934-113">(Örn: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="83934-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="83934-114">Daha fazla bilgi için, [Windows 10 ' da Office 2016 derleme 16.0.7967 güncelleştirmeden sonra oturum açma 'Daki bağlantı sorunlarını](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)izleyin.</span><span class="sxs-lookup"><span data-stu-id="83934-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>