---
title: Parola eşitleme sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664946"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="26ab5-102">Parola eşitleme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="26ab5-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="26ab5-103">Parola eşitleme sorunlarını gidermek için, bu AAD Connect sorun giderme görevini kullanarak parolaların neden eşitlenmediğine karar verin.</span><span class="sxs-lookup"><span data-stu-id="26ab5-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="26ab5-104">Başlamak için [doğrudan Eşitlemeyi Yönet](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)'e gidin.</span><span class="sxs-lookup"><span data-stu-id="26ab5-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="26ab5-105">Azure AD Connect sunucunuzda yeni bir Windows PowerShell oturumu açın ve **yönetici olarak farklı** aç seçeneğini belirtin.</span><span class="sxs-lookup"><span data-stu-id="26ab5-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="26ab5-106">Set-ExecutionPolicy RemoteSigned veya set-ExecutionPolicy kısıtlanmaz.</span><span class="sxs-lookup"><span data-stu-id="26ab5-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="26ab5-107">Azure AD Connect Sihirbazı 'nı başlatın.</span><span class="sxs-lookup"><span data-stu-id="26ab5-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="26ab5-108">Sonraki görevler sayfasına **gidin >**  >  **sonraki**görevler sayfasına gidin.</span><span class="sxs-lookup"><span data-stu-id="26ab5-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="26ab5-109">PowerShell sorun giderme menüsünü açmak için **Başlat** 'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="26ab5-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="26ab5-110">**Parola eşitleme sorunlarını giderme**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="26ab5-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="26ab5-111">Bu sorun genellikle parolanın belirli bir kullanıcı hesabı için eşitlenmemesidir.</span><span class="sxs-lookup"><span data-stu-id="26ab5-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="26ab5-112">**Notları** Son başarılı parola eşitleme işlemi biraz önce olmuşsa parola eşitlemesi başarısız olur.</span><span class="sxs-lookup"><span data-stu-id="26ab5-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="26ab5-113">Parola eşitleme sorunlarını gidermek için, [Azure AD Connect eşitlemesi ile parola karması eşitlemesi sorunlarını giderme](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="26ab5-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>