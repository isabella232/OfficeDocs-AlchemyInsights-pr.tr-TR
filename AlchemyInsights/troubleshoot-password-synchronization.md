---
title: Parola eşitlemesi sorun giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387897"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="5630a-102">Parola eşitlemesi sorun giderme</span><span class="sxs-lookup"><span data-stu-id="5630a-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="5630a-103">Parola eşitleme sorunlarını gidermek için, parolaların neden eşitlenmediğini belirlemek için bu AAD Connect sorun giderme görevini kullanarak başlayın.</span><span class="sxs-lookup"><span data-stu-id="5630a-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="5630a-104">Başlamak için [doğrudan eşitle'yi yönet'e](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)gidin.</span><span class="sxs-lookup"><span data-stu-id="5630a-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="5630a-105">Azure AD Connect sunucunuzda yeni bir Windows PowerShell oturumu açın ve **Yönetici olarak Çalıştır** seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="5630a-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="5630a-106">Set-ExecutionPolicy RemoteSigned veya Set-ExecutionPolicy Sınırsız çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="5630a-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="5630a-107">Azure AD Bağlantısı sihirbazını başlatın.</span><span class="sxs-lookup"><span data-stu-id="5630a-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="5630a-108">Sonraki Sorun **Giderme**> Ek Görevler sayfasına  >  **Next**gidin.</span><span class="sxs-lookup"><span data-stu-id="5630a-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="5630a-109">PowerShell sorun giderme menüsünü açmak için **Başlat'ı** seçin.</span><span class="sxs-lookup"><span data-stu-id="5630a-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="5630a-110">**Sorun Giderme Parola Eşitleme'yi**seçin.</span><span class="sxs-lookup"><span data-stu-id="5630a-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="5630a-111">Sorun genellikle bir parolabelirli bir kullanıcı hesabı için senkronize değildir.</span><span class="sxs-lookup"><span data-stu-id="5630a-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="5630a-112">**Notlar** Son başarılı parola eşitleme bir süre önce yse parola eşitleme başarısız olur.</span><span class="sxs-lookup"><span data-stu-id="5630a-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="5630a-113">Parola eşitleme sorununa yardımcı olmak için Azure [AD Connect eşitlemeyle Sorun Giderme parola karma senkronizasyonu'na](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)bakın.</span><span class="sxs-lookup"><span data-stu-id="5630a-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>