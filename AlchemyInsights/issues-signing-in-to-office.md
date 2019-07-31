---
title: Office uygulamaları için oturum açma sorunları
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938375"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="a8d7d-102">Boş oturum açma ekranı Office apps içinde</span><span class="sxs-lookup"><span data-stu-id="a8d7d-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="a8d7d-103">Bu sorunu gidermek için aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="a8d7d-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="a8d7d-104">[Windows](https://support.microsoft.com/help/4027667/windows-10-update) ve [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)ile ilgili en son güncelleştirmeleri yükleyin.</span><span class="sxs-lookup"><span data-stu-id="a8d7d-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="a8d7d-105">Internet Explorer Seçenekleri sıfırla: **Araçlar** > **Internet Seçenekleri** > **Gelişmiş** > **Internet Explorer Ayarlarını Sıfırla** (özel ayarları kaybedersiniz unutmayın) ve Office için yeniden oturum açmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="a8d7d-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="a8d7d-106">Windows Defender uygulama koruma (WDAG) veya benzer güvenlik duvarı veya virüsten koruma programını devre dışı bırakın:</span><span class="sxs-lookup"><span data-stu-id="a8d7d-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="a8d7d-107">Denetim Masası ' nda **Programlar**gidin ve sonra da **Windows özelliklerini aç veya kapat'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="a8d7d-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="a8d7d-108">Windows Defender uygulama koruyucusu etkinse, devre dışı bırakmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="a8d7d-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="a8d7d-109">**Not:** Bilgisayarı yeniden başlatmanız gerekebilir.</span><span class="sxs-lookup"><span data-stu-id="a8d7d-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="a8d7d-110">Microsoft.AAD.BrokerPlugin [AAD WAM eklenti](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) herhangi bir uygulama veya güvenlik duvarı/anti-virus programı tarafından engelleniyor değil emin olun.</span><span class="sxs-lookup"><span data-stu-id="a8d7d-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="a8d7d-111">Windows kimlik bilgileri yöneticisini kullanarak [Office açık kimlik bilgileri](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .</span><span class="sxs-lookup"><span data-stu-id="a8d7d-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="a8d7d-112">**Not:** Office 2016 için kayıt defteri yolları için 16.0 değişti.</span><span class="sxs-lookup"><span data-stu-id="a8d7d-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="a8d7d-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="a8d7d-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="a8d7d-114">Daha fazla bilgi için bkz: [oturum bileşeninde Office 2016 yapı 16.0.7967 Windows 10 üzerinde güncelleştirme sonra bağlantı sorunları](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="a8d7d-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>