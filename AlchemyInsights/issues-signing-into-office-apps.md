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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579885"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="b08fd-102">Microsoft 365 uygulamalarını düzeltme "Bilgisayarınızın Güvenilir Platform modülü düzgün çalışmıyor" iletisi</span><span class="sxs-lookup"><span data-stu-id="b08fd-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="b08fd-103">Bu hatayı düzeltmek için aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="b08fd-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="b08fd-104">[Windows](https://support.microsoft.com/help/4027667/windows-10-update) ve [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)için en son güncelleştirmeleri yükleyin.</span><span class="sxs-lookup"><span data-stu-id="b08fd-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="b08fd-105">Windows Kimlik Bilgileri Yöneticisi'ni kullanarak [Office kimlik bilgilerini temizleyin.](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)</span><span class="sxs-lookup"><span data-stu-id="b08fd-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="b08fd-106">**Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değiştirildi.</span><span class="sxs-lookup"><span data-stu-id="b08fd-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="b08fd-107">(Ör. \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="b08fd-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="b08fd-108">Güvenilir Platform Modülü (TPM) hatalarını düzeltmek için [kullanıcı kurtarma işlemini](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) deneyin.</span><span class="sxs-lookup"><span data-stu-id="b08fd-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="b08fd-109">Aşağıdaki adımları kullanarak EnableADAL = 0'ı ayarlayın:</span><span class="sxs-lookup"><span data-stu-id="b08fd-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="b08fd-110">Windows Başlat düğmesine sağ tıklayın, **Çalıştır'ı**seçin, **regedit**yazın ve ardından **Tamam'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="b08fd-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="b08fd-111">Kayıt Defteri Düzenleyicisi'nin cihazınızda değişiklik yapmasına izin vermek için **Evet'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="b08fd-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="b08fd-112">Kayıt Defteri Düzenleyicisi'nde, HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity altında **0** ayarı olan **EnableADAL'ın** DWORD değerini ekleyin.</span><span class="sxs-lookup"><span data-stu-id="b08fd-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="b08fd-113">Daha fazla bilgi için bkz: [Windows 10'da Office 2016'da 16.0.7967'yi oluştur'a güncellemeden sonra oturum açma](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)bağlantısı sorunları.</span><span class="sxs-lookup"><span data-stu-id="b08fd-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>