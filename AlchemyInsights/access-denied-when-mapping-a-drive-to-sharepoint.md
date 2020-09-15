---
title: Bir sürücüyü SharePoint ile eşlerken erişim reddedildi
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668763"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="67a77-102">Ağ sürücüleriyle eşlenmiş SharePoint kitaplıkları ile ilgili sorunları giderme</span><span class="sxs-lookup"><span data-stu-id="67a77-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="67a77-103">Eşleşen bir ağ sürücüsüne gözattığınızda, aşağıdaki iletilerden birini görebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="67a77-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="67a77-104">**\\Yol erişilebilir değil. Bu ağ kaynağını kullanma izniniz olmayabilir. Erişim izinleriniz olup olmadığını öğrenmek için bu sunucunun yöneticisine başvurun.**</span><span class="sxs-lookup"><span data-stu-id="67a77-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="67a77-105">**Erişim reddedildi. Bu konumda dosyaları açmadan önce, Web sitesini güvenilen site listenize eklemeniz, Web sitesine gözatmanıza ve otomatik olarak oturum açma seçeneğini işaretlemeniz gerekir.**</span><span class="sxs-lookup"><span data-stu-id="67a77-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="67a77-106">[Eşlenen ağ sürücüleriyle ilgili sorun giderme konusunda yardım alın](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="67a77-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="67a77-107">Kitaplığın ağ sürücüsü olarak eşlenmesi geçicidir ve yalnızca Internet Explorer 'da desteklenir.</span><span class="sxs-lookup"><span data-stu-id="67a77-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="67a77-108">Bunun yerine, SharePoint dosyalarını [isteğe bağlı dosyaları](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)Içeren [yeni OneDrive eşitleme istemcisiyle eşitleyin](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) .</span><span class="sxs-lookup"><span data-stu-id="67a77-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="67a77-109">Yerel depolama alanı kullanmadan OneDrive 'daki tüm dosyalarınıza erişin.</span><span class="sxs-lookup"><span data-stu-id="67a77-109">Access all your files in OneDrive without using local storage space.</span></span>
  