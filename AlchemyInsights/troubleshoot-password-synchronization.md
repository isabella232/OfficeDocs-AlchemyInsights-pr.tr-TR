---
title: Parola eşitleme sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390470"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="930b8-102">Parola eşitleme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="930b8-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="930b8-103">Hiçbir parola Azure AD Connect sürüm 1.1.614.0 ile eşitlenen veya üstü olduğu sorunları gidermek için:</span><span class="sxs-lookup"><span data-stu-id="930b8-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="930b8-104">**Yönetici olarak çalıştır** seçeneğiyle Azure AD Bağlan sunucunuzdaki yeni bir Windows PowerShell oturumu açın.</span><span class="sxs-lookup"><span data-stu-id="930b8-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="930b8-105">**Set-ExecutionPolicy RemoteSigned** veya **Set-ExecutionPolicy sınırsız**çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="930b8-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="930b8-106">Azure AD Bağlan Sihirbazı'nı başlatın.</span><span class="sxs-lookup"><span data-stu-id="930b8-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="930b8-107">Gidin \*\* ek görevler \*\* sayfa, select \*\* giderme \*\*, **İleri**' yi tıklatın.</span><span class="sxs-lookup"><span data-stu-id="930b8-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="930b8-108">Sorun giderme sayfasında PowerShell **sorun giderme işlemlerine başlamak için Başlat** menüsünü tıklatın.</span><span class="sxs-lookup"><span data-stu-id="930b8-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="930b8-109">Ana menüde, **Parola eşitleme sorunlarını giderme**seçin.</span><span class="sxs-lookup"><span data-stu-id="930b8-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="930b8-110">**Parola Eşitleme hiç çalışmıyor**alt menüde seçin.</span><span class="sxs-lookup"><span data-stu-id="930b8-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="930b8-111">**Sorun giderme Görev sonuçlarını anlamak**</span><span class="sxs-lookup"><span data-stu-id="930b8-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="930b8-112">Sorun giderme görev aşağıdaki denetimleri gerçekleştirir:</span><span class="sxs-lookup"><span data-stu-id="930b8-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="930b8-113">Parola eşitleme özelliği, Azure AD Kiracı için etkin olduğunu doğrular.</span><span class="sxs-lookup"><span data-stu-id="930b8-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="930b8-114">Azure AD Connect server hazırlama modu içinde olmadığını doğrular.</span><span class="sxs-lookup"><span data-stu-id="930b8-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="930b8-115">(Varolan bir Active Directory ormanına karşılık gelir) her varolan yerinde Active Directory Bağlayıcısı için:</span><span class="sxs-lookup"><span data-stu-id="930b8-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="930b8-116">Parola eşitleme özelliği etkin olduğunu doğrular.</span><span class="sxs-lookup"><span data-stu-id="930b8-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="930b8-117">Parola eşitleme sinyali olaylar Windows uygulama olay günlüklerine arar.</span><span class="sxs-lookup"><span data-stu-id="930b8-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="930b8-118">Her Active Directory etki alanı için Active Directory Bağlayıcısı yerinde altında:</span><span class="sxs-lookup"><span data-stu-id="930b8-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="930b8-119">Etki alanı AD Bağlan Azure sunucudan ulaşılabilir olduğunu doğrular.</span><span class="sxs-lookup"><span data-stu-id="930b8-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="930b8-120">Şirket içi Active Directory Bağlayıcısı tarafından kullanılan Active Directory etki alanı Hizmetleri (AD DS) hesap doğru kullanıcı adı, parola ve parola eşitleme için gereken izinlere sahip olduğunu doğrular.</span><span class="sxs-lookup"><span data-stu-id="930b8-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="930b8-121">Parola eşitleme sorunlarını giderme hakkında daha fazla yardım için bkz: [eşitleme Azure AD Connect ile parola eşitleme sorunlarını giderme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="930b8-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

