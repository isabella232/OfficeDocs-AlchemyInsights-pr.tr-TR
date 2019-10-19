---
title: SharePoint veya OneDrive'da erişimi kısıtlama
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551471"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="f5196-102">SharePoint veya OneDrive'da erişimi kısıtlama</span><span class="sxs-lookup"><span data-stu-id="f5196-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="f5196-103">SharePoint ve OneDrive'da, yalnızca erişmek istediğiniz gruplara veya kişilere erişim sağlayarak dosya, klasör ve liste gibi öğelere erişimi kısıtlarsınız.</span><span class="sxs-lookup"><span data-stu-id="f5196-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="f5196-104">Varsayılan olarak, SharePoint'teki izinler hiyerarşide yukarıdan devralınır.</span><span class="sxs-lookup"><span data-stu-id="f5196-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="f5196-105">Bu nedenle bir dosya izinlerini siteden alan kitaplıktan izinlerini devralan klasörden devralır.</span><span class="sxs-lookup"><span data-stu-id="f5196-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="f5196-106">Daha yüksek bir düzeyde (örneğin, sitenin tamamını paylaşarak) paylaşabilir ve sitedeki tüm öğeleri paylaşmak istemiyorsanız devralmayı kırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f5196-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="f5196-107">Ancak, izinlerin gelecekte daha karmaşık ve kafa karıştırıcı olmasını sağlar, çünkü bunu önermiyoruz.</span><span class="sxs-lookup"><span data-stu-id="f5196-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="f5196-108">Bunun yerine şunları yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="f5196-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="f5196-109">Örneğin, içinde bir dosya dışında bir klasörün tüm içeriğini paylaşmak istiyorsanız, bu dosyayı paylaşılmamış yeni bir konuma taşıyın.</span><span class="sxs-lookup"><span data-stu-id="f5196-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="f5196-110">Bir klasörde iki alt klasörünüz varsa ve bir alt klasörü A ve B gruplarıyla paylaşmak ve yalnızca A grubu ikinci alt klasöre erişime izin vermek istiyorsanız, ana klasörü A grubuyla paylaşın ve b grubunu ilk alt klasöre ekleyin.</span><span class="sxs-lookup"><span data-stu-id="f5196-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="f5196-111">Dosya veya klasör paylaşımını durdurma</span><span class="sxs-lookup"><span data-stu-id="f5196-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

