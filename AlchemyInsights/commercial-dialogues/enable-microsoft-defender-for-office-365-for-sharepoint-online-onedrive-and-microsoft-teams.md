---
title: SharePoint Online, OneDrive ve Microsoft Teams için Office 365 için Microsoft Defender'ı etkinleştirme
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747737"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="8ff84-102">SharePoint Online, OneDrive ve Microsoft Teams için Office 365 için Microsoft Defender'ı etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="8ff84-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="8ff84-103">Genel yönetici veya güvenlik yöneticisi kimlik bilgilerinizi kullanarak Office 365 Güvenlik ve [Uyumluluk Merkezi'nde oturum açma.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="8ff84-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="8ff84-104">Sol **bölmede Tehdit** yönetimini seçin ve ardından **İlke**  >  [Güvenli eklerini seçin.](https://protection.office.com/safeattachment)</span><span class="sxs-lookup"><span data-stu-id="8ff84-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="8ff84-105">**SharePoint, OneDrive ve Microsoft Teams için Office 365** için Microsoft Defender'ı aç'ı ve ardından Kaydet'i **seçin.**</span><span class="sxs-lookup"><span data-stu-id="8ff84-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="8ff84-106">Genel yönetici veya SharePoint Online yöneticisi olarak, **DisallowInfectedFileDownload** parametresi *true* olarak ayarlanmış aşağıdaki PowerShell cmdlet'ini çalıştırın: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="8ff84-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="8ff84-107">Algılanan dosyalar için uyarıları ayarlama</span><span class="sxs-lookup"><span data-stu-id="8ff84-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="8ff84-108">Daha fazla bilgi için SharePoint, OneDrive ve Microsoft Teams için [Office 365 için Microsoft Defender'a bakın.](https://go.microsoft.com/fwlink/?linkid=2092041)</span><span class="sxs-lookup"><span data-stu-id="8ff84-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
