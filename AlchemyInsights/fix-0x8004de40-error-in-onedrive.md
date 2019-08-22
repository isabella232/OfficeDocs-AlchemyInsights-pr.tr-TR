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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525079"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="162c6-102">OneDrive içinde 0x8004de40 hata düzeltme</span><span class="sxs-lookup"><span data-stu-id="162c6-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="162c6-103">OneDrive ile 0x8004de40 hata alırsanız:</span><span class="sxs-lookup"><span data-stu-id="162c6-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="162c6-104">Acitve Directory etki alanına bağlıyken etkilenen bilgisayarı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="162c6-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="162c6-105">Yeniden başlatma sorunu gidermezse, ayrılma ve aygıtınızdan Azure AD alanına yeniden katın.</span><span class="sxs-lookup"><span data-stu-id="162c6-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="162c6-106">**Not**: aşağıdaki adımları gerçekleştirirken, şirket ağınızda olmalısınız.</span><span class="sxs-lookup"><span data-stu-id="162c6-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="162c6-107">(Örneğin, seyahat ederken) şirket altyapınızı bağlanmak mümkün değildir, bu adımları gerçekleştirmeyin.</span><span class="sxs-lookup"><span data-stu-id="162c6-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="162c6-108">Yükseltilmiş bir komut istemi açın.</span><span class="sxs-lookup"><span data-stu-id="162c6-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="162c6-109">Yükseltilmiş bir komut istemi açmak için **Başlat**' ı tıklatın -, **komut istemini**sağ tıklatın ve sonra **yönetici olarak çalıştır**' ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="162c6-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="162c6-110">*Dsregcmd /leave* yazın ve **Enter**tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="162c6-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="162c6-111">Tamamlandığında, *dsregcmd /join* yazın ve **Enter**tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="162c6-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="162c6-112">Tamamlandığında komut istemini kapatın.</span><span class="sxs-lookup"><span data-stu-id="162c6-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="162c6-113">Bilgisayarı yeniden başlatıp oturum OneDrive.</span><span class="sxs-lookup"><span data-stu-id="162c6-113">Reboot the computer, and log into OneDrive.</span></span>