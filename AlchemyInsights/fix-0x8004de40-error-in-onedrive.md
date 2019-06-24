---
title: OneDrive içinde 0x8004de40 hata düzeltme
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133996"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="db138-102">OneDrive içinde 0x8004de40 hata düzeltme</span><span class="sxs-lookup"><span data-stu-id="db138-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="db138-103">OneDrive ile 0x8004de40 hata alırsanız:</span><span class="sxs-lookup"><span data-stu-id="db138-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="db138-104">Acitve Directory etki alanına bağlıyken etkilenen bilgisayarı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="db138-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="db138-105">Yeniden başlatma sorunu gidermezse, ayrılma ve aygıtınızdan Azure AD alanına yeniden katın.</span><span class="sxs-lookup"><span data-stu-id="db138-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="db138-106">**Not**: aşağıdaki adımları gerçekleştirirken, şirket ağınızda olmalısınız.</span><span class="sxs-lookup"><span data-stu-id="db138-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="db138-107">(Örneğin, seyahat ederken) şirket altyapınızı bağlanmak mümkün değildir, bu adımları gerçekleştirmeyin.</span><span class="sxs-lookup"><span data-stu-id="db138-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="db138-108">Yükseltilmiş bir komut istemi açın.</span><span class="sxs-lookup"><span data-stu-id="db138-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="db138-109">Yükseltilmiş bir komut istemi açmak için **Başlat**' ı tıklatın -, **komut istemini**sağ tıklatın ve sonra **yönetici olarak çalıştır**' ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="db138-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="db138-110">*Dsregcmd /leave* yazın ve **Enter**tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="db138-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="db138-111">Tamamlandığında, *dsregcmd /join* yazın ve **Enter**tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="db138-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="db138-112">Tamamlandığında komut istemini kapatın.</span><span class="sxs-lookup"><span data-stu-id="db138-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="db138-113">Bilgisayarı yeniden başlatıp oturum OneDrive.</span><span class="sxs-lookup"><span data-stu-id="db138-113">Reboot the computer, and log into OneDrive.</span></span>