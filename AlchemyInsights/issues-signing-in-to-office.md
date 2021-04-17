---
title: Microsoft 365 uygulamalarına oturum açma sorunları
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833059"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="20b34-102">Microsoft 365 uygulamalarında boş oturum açma ekranı</span><span class="sxs-lookup"><span data-stu-id="20b34-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="20b34-103">Bu sorunu çözmek için şunları deneyin:</span><span class="sxs-lookup"><span data-stu-id="20b34-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="20b34-104">Windows ve Office için en [son güncelleştirmeleri](https://support.microsoft.com/help/4027667/windows-10-update) [yükleyin.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="20b34-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="20b34-105">Internet Explorer seçeneklerini sıfırlama: Araçlar Internet Seçenekleri Gelişmiş Internet Explorer Ayarlarını Sıfırla 'ya gidin (özel ayarları kaybedeceğinizi unutmayın) ve Office'te oturum  >    >    >   açmayı yeniden deneyin.</span><span class="sxs-lookup"><span data-stu-id="20b34-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="20b34-106">Windows Defender Application Guard'ı (WDAG) veya benzer güvenlik duvarını veya virüsten koruma programını devre dışı bırakma:</span><span class="sxs-lookup"><span data-stu-id="20b34-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="20b34-107">Denetim Masası'nda **Programlar'a gidin** ve Windows özelliklerini **aç veya kapat'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="20b34-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="20b34-108">Windows Defender Application Guard etkinleştirildiyse, bu özelliği devre dışı bırakmayı deneyin.</span><span class="sxs-lookup"><span data-stu-id="20b34-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="20b34-109">**Not:** Bilgisayarı yeniden başlatmanız gerekiyor olabilir.</span><span class="sxs-lookup"><span data-stu-id="20b34-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="20b34-110">Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) eklentisinin herhangi bir uygulama veya güvenlik duvarı/virüsten koruma programı tarafından engelli olmadığını kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="20b34-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="20b34-111">Windows [Kimlik Bilgileri Yöneticisi'ni](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) kullanarak Office kimlik bilgilerini temizleme.</span><span class="sxs-lookup"><span data-stu-id="20b34-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="20b34-112">**Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değişti.</span><span class="sxs-lookup"><span data-stu-id="20b34-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="20b34-113">(Örneğin: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="20b34-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="20b34-114">Daha fazla bilgi için [bkz. Windows 10 üzerinde Office 2016 derleme 16.0.7967'ye](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)güncelleştirdikten sonra oturum açma işlemiyle ilgili bağlantı sorunları.</span><span class="sxs-lookup"><span data-stu-id="20b34-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>