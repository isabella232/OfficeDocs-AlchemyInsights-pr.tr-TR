---
title: OneDrive'da 0x8004de40 hatasini düzeltin
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716048"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="f1516-102">OneDrive'da 0x8004de40 hatasini düzeltin</span><span class="sxs-lookup"><span data-stu-id="f1516-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="f1516-103">OneDrive ile 0x8004de40 hatası alırsanız:</span><span class="sxs-lookup"><span data-stu-id="f1516-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="f1516-104">Acitve Directory etki alanınıza bağlıyken etkilenen bilgisayarı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="f1516-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="f1516-105">Yeniden başlatma sorunu çözmezse, Azure AD'den cihazınıza katılın ve yeniden katılın.</span><span class="sxs-lookup"><span data-stu-id="f1516-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="f1516-106">**Not**: Bu adımları gerçekleştirirken şirket ağınızda olmalısınız.</span><span class="sxs-lookup"><span data-stu-id="f1516-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="f1516-107">Kurumsal altyapınıza bağlanamadığınızda (örneğin, seyahat ederken) bu adımları gerçekleştirin.</span><span class="sxs-lookup"><span data-stu-id="f1516-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="f1516-108">Yükseltilmiş bir komut istemini açın.</span><span class="sxs-lookup"><span data-stu-id="f1516-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="f1516-109">Yükseltilmiş komut istemini açmak için - **Başlat,** **Komut İstem'i**sağ tıklatın ve ardından **yönetici olarak çalıştır'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="f1516-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="f1516-110">*Dsregcmd* yazın /bırak ve **Enter**tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="f1516-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="f1516-111">Tamamlandığında, *dsregcmd yazın /join* ve **Enter**tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="f1516-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="f1516-112">Tamamlandığında, komut istemini kapatın.</span><span class="sxs-lookup"><span data-stu-id="f1516-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="f1516-113">Bilgisayarı yeniden başlatın ve OneDrive'a giriş yapın.</span><span class="sxs-lookup"><span data-stu-id="f1516-113">Reboot the computer, and log into OneDrive.</span></span>