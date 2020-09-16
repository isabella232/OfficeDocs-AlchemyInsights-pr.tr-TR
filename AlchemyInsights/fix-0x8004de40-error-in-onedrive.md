---
title: OneDrive 'da 0x8004de40 hatasını düzeltme
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745150"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="8d954-102">OneDrive 'da 0x8004de40 hatasını düzeltme</span><span class="sxs-lookup"><span data-stu-id="8d954-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="8d954-103">OneDrive ile bir 0x8004de40 hatası alıyorsanız:</span><span class="sxs-lookup"><span data-stu-id="8d954-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="8d954-104">Acitve dizin etki alanınıza bağlıyken etkilenen bilgisayarı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="8d954-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="8d954-105">Yeniden yükleme sorunu çözmezse, aboneliğinizi kaldırın ve cihazınızı Azure AD 'den yeniden katın.</span><span class="sxs-lookup"><span data-stu-id="8d954-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="8d954-106">**Not**: Bu adımları uygularken şirket ağınızda olmalısınız.</span><span class="sxs-lookup"><span data-stu-id="8d954-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="8d954-107">Şirket altyapısına (örneğin, seyahat halindeyken) bağlanamadığınızda bu adımları kullanmayın.</span><span class="sxs-lookup"><span data-stu-id="8d954-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="8d954-108">Yükseltilmiş bir komut istemi açın.</span><span class="sxs-lookup"><span data-stu-id="8d954-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="8d954-109">Yükseltilmiş bir komut istemini açmak için- **Başlat**'a tıklayın, **komut istemi**'ne sağ tıklayın ve **yönetici olarak Run**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="8d954-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="8d954-110">*Dsregcmd/Leave* yazın ve **ENTER**tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="8d954-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="8d954-111">Tamamlandığında *dsregcmd/Join* yazın ve **ENTER**tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="8d954-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="8d954-112">Tamamlandığında komut istemini kapatın.</span><span class="sxs-lookup"><span data-stu-id="8d954-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="8d954-113">Bilgisayarı yeniden başlatın ve OneDrive 'da oturum açın.</span><span class="sxs-lookup"><span data-stu-id="8d954-113">Reboot the computer, and log into OneDrive.</span></span>