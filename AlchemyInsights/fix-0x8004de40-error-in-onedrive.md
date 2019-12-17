---
title: OneDrive'da 0x8004de40 hatasini düzeltin
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052057"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="4e4ad-102">OneDrive'da 0x8004de40 hatasini düzeltin</span><span class="sxs-lookup"><span data-stu-id="4e4ad-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="4e4ad-103">OneDrive ile 0x8004de40 hatası alırsanız:</span><span class="sxs-lookup"><span data-stu-id="4e4ad-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="4e4ad-104">Acitve Directory etki alanınıza bağlıyken etkilenen bilgisayarı yeniden başlatın.</span><span class="sxs-lookup"><span data-stu-id="4e4ad-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="4e4ad-105">Yeniden başlatma sorunu çözmezse, Azure AD'den cihazınıza katılın ve yeniden katılın.</span><span class="sxs-lookup"><span data-stu-id="4e4ad-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="4e4ad-106">**Not**: Bu adımları gerçekleştirirken şirket ağınızda olmalısınız.</span><span class="sxs-lookup"><span data-stu-id="4e4ad-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="4e4ad-107">Kurumsal altyapınıza bağlanamadığınızda (örneğin, seyahat ederken) bu adımları gerçekleştirin.</span><span class="sxs-lookup"><span data-stu-id="4e4ad-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="4e4ad-108">Yükseltilmiş bir komut istemini açın.</span><span class="sxs-lookup"><span data-stu-id="4e4ad-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="4e4ad-109">Yükseltilmiş komut istemini açmak için - **Başlat,** **Komut İstem'i**sağ tıklatın ve ardından **yönetici olarak çalıştır'ı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="4e4ad-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="4e4ad-110">*Dsregcmd* yazın /bırak ve **Enter**tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="4e4ad-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="4e4ad-111">Tamamlandığında, *dsregcmd yazın /join* ve **Enter**tuşuna basın.</span><span class="sxs-lookup"><span data-stu-id="4e4ad-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="4e4ad-112">Tamamlandığında, komut istemini kapatın.</span><span class="sxs-lookup"><span data-stu-id="4e4ad-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="4e4ad-113">Bilgisayarı yeniden başlatın ve OneDrive'a giriş yapın.</span><span class="sxs-lookup"><span data-stu-id="4e4ad-113">Reboot the computer, and log into OneDrive.</span></span>