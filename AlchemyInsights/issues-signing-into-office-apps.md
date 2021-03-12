---
title: Microsoft 365 uygulamalarına oturum açma sorunları
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
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709126"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="7428c-102">Microsoft 365 uygulamalarını düzeltme "Bilgisayarınızın Güvenilen Platform modülü düzgün çalışmıyor" iletisi</span><span class="sxs-lookup"><span data-stu-id="7428c-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="7428c-103">Bu hatayı düzeltmek için aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="7428c-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="7428c-104">Windows ve Office'in en [son güncelleştirmelerini](https://support.microsoft.com/help/4027667/windows-10-update) [yükleyin.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="7428c-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="7428c-105">Windows [Kimlik Bilgileri Yöneticisi'ni](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) kullanarak Office kimlik bilgilerini temizleme.</span><span class="sxs-lookup"><span data-stu-id="7428c-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="7428c-106">**Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değiştirildi.</span><span class="sxs-lookup"><span data-stu-id="7428c-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="7428c-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="7428c-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="7428c-108">Güvenilen Platform [Modülü](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) (TPM) hatalarını düzeltmek için kullanıcı kurtarma işlemini deneyin.</span><span class="sxs-lookup"><span data-stu-id="7428c-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="7428c-109">Aşağıdaki adımları kullanarak EnableADAL = 0'ı ayarlayın:</span><span class="sxs-lookup"><span data-stu-id="7428c-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="7428c-110">Windows Başlat düğmesine sağ tıklayın, Çalıştır'ı **seçin,** **regedit yazın** ve Tamam'ı **seçin.**</span><span class="sxs-lookup"><span data-stu-id="7428c-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="7428c-111">Kayıt **Defteri Düzenleyicisi'nin** aygıtınızda değişiklik yapmalarına izin vermek için Evet'i seçin.</span><span class="sxs-lookup"><span data-stu-id="7428c-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="7428c-112">Kayıt Defteri Düzenleyicisi'nde, **0** ayarıyla **EnableADAL'ın** DWORD değerini HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="7428c-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="7428c-113">Daha fazla bilgi için, [Windows 10'da Office 2016 derleme 16.0.7967'ye](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)güncelleştirme sonrasında oturum açmayla ilgili bağlantı sorunlarına bakın.</span><span class="sxs-lookup"><span data-stu-id="7428c-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>