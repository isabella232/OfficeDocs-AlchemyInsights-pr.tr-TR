---
title: ClientAccessServerEnabled'ı True olarak ayarlama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527417"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="bd233-102">ClientAccessServerEnabled'ı True olarak ayarlama</span><span class="sxs-lookup"><span data-stu-id="bd233-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="bd233-103">Şifreli bir e-posta iletisini açasanız ve bunun yerine **bir rpmsg** eki görüyorsanız, aşağıdaki adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="bd233-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="bd233-104">Exchange Online PowerShell'e bağlanın.</span><span class="sxs-lookup"><span data-stu-id="bd233-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="bd233-105">Exchange Online PowerShell'e bağlanmak için genel yönetici veya Exchange yönetici hesabıyla oturum açın.</span><span class="sxs-lookup"><span data-stu-id="bd233-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="bd233-106">a.</span><span class="sxs-lookup"><span data-stu-id="bd233-106">a.</span></span> <span data-ttu-id="bd233-107">Windows PowerShell'i açın ve sonra aşağıdaki komutu çalıştırın: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="bd233-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="bd233-108">b.</span><span class="sxs-lookup"><span data-stu-id="bd233-108">b.</span></span> <span data-ttu-id="bd233-109">Windows **PowerShell Kimlik Bilgileri İsteği** iletişim kutusuna iş veya okul hesabınızla parolanızı girin, c.</span><span class="sxs-lookup"><span data-stu-id="bd233-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="bd233-110">**Tamam**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="bd233-110">Click **OK**.</span></span> 

2. <span data-ttu-id="bd233-111">Yeni bir oturum oluşturmak için aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="bd233-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="bd233-112">a.</span><span class="sxs-lookup"><span data-stu-id="bd233-112">a.</span></span> <span data-ttu-id="bd233-113">Aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="bd233-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="bd233-114">Çalıştır `Get-IRMConfiguration` komutu.</span><span class="sxs-lookup"><span data-stu-id="bd233-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="bd233-115">**ClientAccessServerEnabled ayarını** kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="bd233-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="bd233-116">a.</span><span class="sxs-lookup"><span data-stu-id="bd233-116">a.</span></span> <span data-ttu-id="bd233-117">**ClientAccessServerEnabled** ayarı False olarak **ayarlanmışsa,** aşağıdaki cmdlet'i çalıştırın:`Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="bd233-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="bd233-118">Her zaman aşağıdaki komutu kullanarak PowerShell oturumlarınızı kapatın: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="bd233-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="bd233-119">Daha fazla bilgi için [bkz. Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="bd233-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

