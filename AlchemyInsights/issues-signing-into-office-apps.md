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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695199"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="23c8c-102">Microsoft 365 uygulamalarının "bilgisayarınızın Güvenilir Platform Modülü düzgün çalışmıyor" iletisini Düzeltme</span><span class="sxs-lookup"><span data-stu-id="23c8c-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="23c8c-103">Bu hatayı düzeltmek için aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="23c8c-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="23c8c-104">En son [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ve [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)güncelleştirmelerini yükleyin.</span><span class="sxs-lookup"><span data-stu-id="23c8c-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="23c8c-105">Windows kimlik bilgileri Yöneticisi 'Ni kullanarak [Office kimlik bilgilerini temizleyin](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .</span><span class="sxs-lookup"><span data-stu-id="23c8c-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="23c8c-106">**Not:** Office 2016 için kayıt defteri yolları 16,0 olarak değiştirilmiştir.</span><span class="sxs-lookup"><span data-stu-id="23c8c-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="23c8c-107">(Örn: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="23c8c-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="23c8c-108">Güvenilir Platform Modülü (TPM) hatalarını düzeltmek için [Kullanıcı kurtarma işlemini](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) deneyin.</span><span class="sxs-lookup"><span data-stu-id="23c8c-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="23c8c-109">Aşağıdaki adımları kullanarak EnableADAL = 0 değerini ayarlayın:</span><span class="sxs-lookup"><span data-stu-id="23c8c-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="23c8c-110">Windows Başlat düğmesine sağ **tıklayın, Başlat 'ı seçin,** **Regedit**yazın ve **Tamam**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="23c8c-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="23c8c-111">Kayıt Defteri Düzenleyicisi 'nin cihazınızda değişiklik yapmasına izin vermek için **Evet 'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="23c8c-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="23c8c-112">Kayıt Defteri Düzenleyicisi 'nde, HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity. altındaki **0** ayarına sahip **ENABLEADAL** DWORD değerini ekleyin</span><span class="sxs-lookup"><span data-stu-id="23c8c-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="23c8c-113">Daha fazla bilgi için, [Windows 10 ' da Office 2016 derleme 16.0.7967 güncelleştirmeden sonra oturum açma 'Daki bağlantı sorunlarını](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)izleyin.</span><span class="sxs-lookup"><span data-stu-id="23c8c-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>