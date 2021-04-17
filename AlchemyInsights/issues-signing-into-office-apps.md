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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833035"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="5ed5a-102">Microsoft 365 uygulamaları "Bilgisayarınızın Güvenilen Platform modülü düzgün çalışmıyor" iletisi düzeltme</span><span class="sxs-lookup"><span data-stu-id="5ed5a-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="5ed5a-103">Bu hatayı düzeltmek için aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="5ed5a-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="5ed5a-104">Windows ve Office için en [son güncelleştirmeleri](https://support.microsoft.com/help/4027667/windows-10-update) [yükleyin.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="5ed5a-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="5ed5a-105">Windows [Kimlik Bilgileri Yöneticisi'ni](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) kullanarak Office kimlik bilgilerini temizleme.</span><span class="sxs-lookup"><span data-stu-id="5ed5a-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="5ed5a-106">**Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değişti.</span><span class="sxs-lookup"><span data-stu-id="5ed5a-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="5ed5a-107">(Örneğin: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="5ed5a-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="5ed5a-108">Güvenilir Platform [Modülü](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) (TPM) hatalarını düzeltmek için kullanıcı kurtarma işlemini deneyin.</span><span class="sxs-lookup"><span data-stu-id="5ed5a-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="5ed5a-109">Aşağıdaki adımları kullanarak EnableADAL = 0 ayarlayın:</span><span class="sxs-lookup"><span data-stu-id="5ed5a-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="5ed5a-110">Windows Başlat düğmesine sağ tıklayın, Çalıştır'ı **seçin,** **regedit yazın ve** ardından Tamam'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="5ed5a-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="5ed5a-111">Kayıt **Defteri Düzenleyicisi'nin** aygıtınızda değişiklik yapmalarına izin vermek için Evet'i seçin.</span><span class="sxs-lookup"><span data-stu-id="5ed5a-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="5ed5a-112">Kayıt Defteri Düzenleyicisi'nde, Düzenleyici'nin altında **0** değeriyle **EnableADAL** için DWORD HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="5ed5a-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="5ed5a-113">Daha fazla bilgi için [bkz. Windows 10 üzerinde Office 2016 derleme 16.0.7967'ye](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)güncelleştirdikten sonra oturum açma işlemiyle ilgili bağlantı sorunları.</span><span class="sxs-lookup"><span data-stu-id="5ed5a-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>