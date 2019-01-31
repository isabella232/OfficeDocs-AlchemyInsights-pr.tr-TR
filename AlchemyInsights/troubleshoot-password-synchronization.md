---
title: Parola eşitleme sorunlarını giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 589820c945fb20f00431655f9f53196e740bb38f
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655831"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="55005-102">Parola eşitleme sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="55005-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="55005-103">Hiçbir parola Azure AD Connect sürüm 1.1.614.0 ile eşitlenen veya üstü olduğu sorunları gidermek için:</span><span class="sxs-lookup"><span data-stu-id="55005-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="55005-104">**Yönetici olarak çalıştır** seçeneğiyle Azure AD Bağlan sunucunuzdaki yeni bir Windows PowerShell oturumu açın.</span><span class="sxs-lookup"><span data-stu-id="55005-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="55005-105">**Set-ExecutionPolicy RemoteSigned** veya **Set-ExecutionPolicy sınırsız**çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="55005-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="55005-106">Azure AD Bağlan Sihirbazı'nı başlatın.</span><span class="sxs-lookup"><span data-stu-id="55005-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="55005-107">Gidin \*\* ek görevler \*\* sayfa, select \*\* giderme \*\*, **İleri**' yi tıklatın.</span><span class="sxs-lookup"><span data-stu-id="55005-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="55005-108">Sorun giderme sayfasında PowerShell **sorun giderme işlemlerine başlamak için Başlat** menüsünü tıklatın.</span><span class="sxs-lookup"><span data-stu-id="55005-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="55005-109">Ana menüde, **Parola eşitleme sorunlarını giderme**seçin.</span><span class="sxs-lookup"><span data-stu-id="55005-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="55005-110">**Parola Eşitleme hiç çalışmıyor**alt menüde seçin.</span><span class="sxs-lookup"><span data-stu-id="55005-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="55005-111">**Sorun giderme Görev sonuçlarını anlamak**</span><span class="sxs-lookup"><span data-stu-id="55005-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="55005-112">Sorun giderme görev aşağıdaki denetimleri gerçekleştirir:</span><span class="sxs-lookup"><span data-stu-id="55005-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="55005-113">Parola eşitleme özelliği, Azure AD Kiracı için etkin olduğunu doğrular.</span><span class="sxs-lookup"><span data-stu-id="55005-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="55005-114">Azure AD Connect server hazırlama modu içinde olmadığını doğrular.</span><span class="sxs-lookup"><span data-stu-id="55005-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="55005-115">(Varolan bir Active Directory ormanına karşılık gelir) her varolan yerinde Active Directory Bağlayıcısı için:</span><span class="sxs-lookup"><span data-stu-id="55005-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="55005-116">Parola eşitleme özelliği etkin olduğunu doğrular.</span><span class="sxs-lookup"><span data-stu-id="55005-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="55005-117">Parola eşitleme sinyali olaylar Windows uygulama olay günlüklerine arar.</span><span class="sxs-lookup"><span data-stu-id="55005-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="55005-118">Her Active Directory etki alanı için Active Directory Bağlayıcısı yerinde altında:</span><span class="sxs-lookup"><span data-stu-id="55005-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="55005-119">Etki alanı AD Bağlan Azure sunucudan ulaşılabilir olduğunu doğrular.</span><span class="sxs-lookup"><span data-stu-id="55005-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="55005-120">Şirket içi Active Directory Bağlayıcısı tarafından kullanılan Active Directory etki alanı Hizmetleri (AD DS) hesap doğru kullanıcı adı, parola ve parola eşitleme için gereken izinlere sahip olduğunu doğrular.</span><span class="sxs-lookup"><span data-stu-id="55005-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="55005-121">Parola eşitleme sorunlarını giderme hakkında daha fazla yardım için bkz: [eşitleme Azure AD Connect ile parola eşitleme sorunlarını giderme](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="55005-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

