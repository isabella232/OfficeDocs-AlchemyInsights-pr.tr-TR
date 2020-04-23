---
title: Parola eşitlemesi sorun giderme
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732530"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="1b22a-102">Parola eşitlemesi sorun giderme</span><span class="sxs-lookup"><span data-stu-id="1b22a-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="1b22a-103">Azure AD Connect sürümü 1.1.614.0 veya sonraki sürümle hiçbir parolanın eşitlenmediği sorunları gidermek için:</span><span class="sxs-lookup"><span data-stu-id="1b22a-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="1b22a-104">Azure AD Connect sunucunuzda **Yönetici olarak Çalıştır** seçeneğiyle yeni bir Windows PowerShell oturumu açın.</span><span class="sxs-lookup"><span data-stu-id="1b22a-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="1b22a-105">**Set-ExecutionPolicy RemoteSigned** veya **Set-ExecutionPolicy Sınırsız**çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="1b22a-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="1b22a-106">Azure AD Bağlantısı sihirbazını başlatın.</span><span class="sxs-lookup"><span data-stu-id="1b22a-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="1b22a-107">**Ek Görevler** sayfasına gidin, **Sorun Giderme'yi**seçin ve **İleri'yi**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="1b22a-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="1b22a-108">Sorun Giderme sayfasında, **PowerShell'deki sorun giderme menüsünü başlatmak için Başlat'ı** tıklatın.</span><span class="sxs-lookup"><span data-stu-id="1b22a-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="1b22a-109">Ana menüde **Sorun Giderme Parola Eşitlemesi'ni**seçin.</span><span class="sxs-lookup"><span data-stu-id="1b22a-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="1b22a-110">Alt menüde **Parola Eşitlemesi'ni**seçin hiç çalışmıyor.</span><span class="sxs-lookup"><span data-stu-id="1b22a-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="1b22a-111">**Sorun giderme görevinin sonuçlarını anlama**</span><span class="sxs-lookup"><span data-stu-id="1b22a-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="1b22a-112">Sorun giderme görevi aşağıdaki denetimleri gerçekleştirir:</span><span class="sxs-lookup"><span data-stu-id="1b22a-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="1b22a-113">Azure AD kiracınız için parola eşitleme özelliğinin etkin olduğunu doğrular.</span><span class="sxs-lookup"><span data-stu-id="1b22a-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="1b22a-114">Azure AD Connect sunucusunun hazırlama modunda olmadığını doğrular.</span><span class="sxs-lookup"><span data-stu-id="1b22a-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="1b22a-115">Varolan her şirket içi Active Directory bağlayıcısı için (varolan bir Active Directory ormanına karşılık gelir):</span><span class="sxs-lookup"><span data-stu-id="1b22a-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="1b22a-116">Parola eşitleme özelliğinin etkin olduğunu doğrular.</span><span class="sxs-lookup"><span data-stu-id="1b22a-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="1b22a-117">Windows Application Event günlüklerinde parola eşitleme sinyali olaylarını arar.</span><span class="sxs-lookup"><span data-stu-id="1b22a-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="1b22a-118">Şirket içi Active Directory bağlayıcısı altındaki her Active Directory etki alanı için:</span><span class="sxs-lookup"><span data-stu-id="1b22a-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="1b22a-119">Etki alanına Azure AD Connect sunucusundan erişilebildiğini doğrular.</span><span class="sxs-lookup"><span data-stu-id="1b22a-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="1b22a-120">Şirket içi Active Directory bağlayıcısı tarafından kullanılan Active Directory Domain Services (AD DS) hesaplarının parola eşitleme için gereken doğru kullanıcı adı, parola ve izinlere sahip olduğunu doğrular.</span><span class="sxs-lookup"><span data-stu-id="1b22a-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="1b22a-121">Parola eşitleme sorununa yardımcı olmak için Azure [AD Connect eşitlemeyle Sorun Giderme Parola senkronizasyonu'na](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)bakın.</span><span class="sxs-lookup"><span data-stu-id="1b22a-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  