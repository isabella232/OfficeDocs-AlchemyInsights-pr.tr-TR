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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938376"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="c0c02-102">Office uygulamaları "bilgisayarınızın Güvenilen Platform Modülü düzgün çalışmıyor" iletisini çözme</span><span class="sxs-lookup"><span data-stu-id="c0c02-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="c0c02-103">Bu hatayı düzeltmek için aşağıdakileri deneyin:</span><span class="sxs-lookup"><span data-stu-id="c0c02-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="c0c02-104">[Windows](https://support.microsoft.com/help/4027667/windows-10-update) ve [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)ile ilgili en son güncelleştirmeleri yükleyin.</span><span class="sxs-lookup"><span data-stu-id="c0c02-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="c0c02-105">Windows kimlik bilgileri yöneticisini kullanarak [Office açık kimlik bilgileri](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .</span><span class="sxs-lookup"><span data-stu-id="c0c02-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="c0c02-106">**Not:** Office 2016 için kayıt defteri yolları için 16.0 değişti.</span><span class="sxs-lookup"><span data-stu-id="c0c02-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="c0c02-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="c0c02-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="c0c02-108">Güvenilir Platform Modülü (TPM) hataları düzeltmek için [kullanıcı kurtarma işlemi](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) deneyin.</span><span class="sxs-lookup"><span data-stu-id="c0c02-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="c0c02-109">Set EnableADAL = 0 aşağıdaki adımları kullanarak:</span><span class="sxs-lookup"><span data-stu-id="c0c02-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="c0c02-110">Windows Başlat düğmesini sağ tıklatın, **Çalıştır**' ı seçin, **regedit**yazın ve **Tamam**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="c0c02-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="c0c02-111">Kayıt Defteri Düzenleyicisi, aygıtınız için değişiklik yapmak için izin vermek için **Evet** ' i seçin.</span><span class="sxs-lookup"><span data-stu-id="c0c02-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="c0c02-112">Kayıt Defteri Düzenleyicisi'nde bir ayarı **0** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity altında **EnableADAL** DWORD değerini ekleyin.</span><span class="sxs-lookup"><span data-stu-id="c0c02-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="c0c02-113">Daha fazla bilgi için bkz: [oturum bileşeninde Office 2016 yapı 16.0.7967 Windows 10 üzerinde güncelleştirme sonra bağlantı sorunları](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="c0c02-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>