---
title: SharePoint veya OneDrive 'da erişimi kısıtlama
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720702"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="d6a95-102">SharePoint veya OneDrive 'da erişimi kısıtlama</span><span class="sxs-lookup"><span data-stu-id="d6a95-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="d6a95-103">SharePoint ve OneDrive 'da, yalnızca erişmek istediğiniz gruplara veya kişilere erişim vererek dosyalar, klasörler ve listeler gibi öğelere erişimi kısıtlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d6a95-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="d6a95-104">Varsayılan olarak, SharePoint 'teki izinler hiyerarşide daha yüksek bir düzeye devralınır.</span><span class="sxs-lookup"><span data-stu-id="d6a95-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="d6a95-105">Böylece, bir dosya kendi izinlerini veritabanından devralır ve bu da sunucudaki izinleri veritabanından devralır.</span><span class="sxs-lookup"><span data-stu-id="d6a95-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="d6a95-106">Daha yüksek düzeyde paylaşım yapabilirsiniz (tüm siteyi paylaşabilir gibi) ve sonra sitedeki tüm öğeleri paylaşmak istemezseniz devralmayı bozabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d6a95-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="d6a95-107">Bununla birlikte, daha sonra izinlerin daha karmaşık ve kafa karıştırıcı olduğundan bunu önermiyoruz.</span><span class="sxs-lookup"><span data-stu-id="d6a95-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="d6a95-108">Bunun yerine yapabilecekleriniz:</span><span class="sxs-lookup"><span data-stu-id="d6a95-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="d6a95-109">Örneğin, bir dosya dışında bir klasörün tüm içeriğini paylaşmak istiyorsanız, dosyayı paylaşılmayan yeni bir konuma taşıyın.</span><span class="sxs-lookup"><span data-stu-id="d6a95-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="d6a95-110">Bir klasörde iki alt klasörünüz varsa ve yalnızca A ve B gruplarıyla tek bir alt klasör paylaşmak istiyorsanız ve ikinci alt klasöre yalnızca Grup erişimi izni vermek istiyorsanız, ana klasörü grupla ve Grup B 'yi ilk alt klasöre paylaşın.</span><span class="sxs-lookup"><span data-stu-id="d6a95-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="d6a95-111">Dosya veya klasör paylaşmayı durdurma </span><span class="sxs-lookup"><span data-stu-id="d6a95-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

