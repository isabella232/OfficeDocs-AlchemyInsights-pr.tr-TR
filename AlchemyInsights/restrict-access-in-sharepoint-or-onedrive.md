---
title: SharePoint veya OneDrive erişimi sınırlama
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551471"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="b6517-102">SharePoint veya OneDrive erişimi sınırlama</span><span class="sxs-lookup"><span data-stu-id="b6517-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="b6517-103">SharePoint ve OneDrive, dosyalar, klasörler ve listeleri gibi maddelere erişimi vererek, yalnızca grupların veya kişilerin erişimi olmasını istediğiniz için erişimi.</span><span class="sxs-lookup"><span data-stu-id="b6517-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="b6517-104">Varsayılan olarak, SharePoint izinleri sıradüzeninde daha yüksek up dan devralınır.</span><span class="sxs-lookup"><span data-stu-id="b6517-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="b6517-105">Bu nedenle dosya izinlerini siteden devralan kitaplığı izinlerini devralır klasöründen kendi izinleri devralır.</span><span class="sxs-lookup"><span data-stu-id="b6517-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="b6517-106">Daha yüksek bir düzeyde paylaşabilirsiniz (gibi tüm bir siteyi paylaşımı tarafından) ve sitedeki tüm öğeleri paylaşmak istemiyorsanız, sonra devralma bölün.</span><span class="sxs-lookup"><span data-stu-id="b6517-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="b6517-107">İzinleri daha karmaşık ve kafa karıştırıcı gelecekte bakımını yapar çünkü ancak, bu önermemekteyiz.</span><span class="sxs-lookup"><span data-stu-id="b6517-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="b6517-108">İşte bunun yerine ne:</span><span class="sxs-lookup"><span data-stu-id="b6517-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="b6517-109">Örneğin, bir klasörü dışında bir dosyada tüm içeriğini paylaşmak istiyorsanız bu dosyayı paylaşılan olmayan yeni bir konuma taşıyın.</span><span class="sxs-lookup"><span data-stu-id="b6517-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="b6517-110">Bir klasördeki iki altklasörü olan ve bir alt klasör grupları A ve B paylaşmak ve yalnızca ikinci alt grubu A erişim izni, A grubu ile üst klasörü paylaşmak ve B grubu için ilk alt klasörü eklemek istediğiniz varsa.</span><span class="sxs-lookup"><span data-stu-id="b6517-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="b6517-111">Bir dosya veya klasörün paylaşımını durdurma</span><span class="sxs-lookup"><span data-stu-id="b6517-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

