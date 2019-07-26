---
title: Ad Sunucularını Değiştirme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f4b5001f2a6291a422b5cd0c3c40de7be0f1ecf0
ms.sourcegitcommit: 20b6a1fb3f0d899f3b204e3c066262d10623a4ea
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35902949"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="201cb-102">Etki alanı ad sunucularınızı Office 365'e güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="201cb-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="201cb-103">Not: Ad sunucusu değişikliklerinin yayılması bazen 48 saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="201cb-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="201cb-p101">Office 365’te etki alanınızı ayarlamak için kayıt şirketinizdeki ad sunucularının güncelleştirilmesi gerekir. Etki alanı kayıt şirketinizde ad sunucusu kayıtlarınızı oluşturun veya düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="201cb-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="201cb-106">Etki alanı kayıt şirketinizin web sitesine gidin ve ad sunucularını düzenleyebileceğiniz alanı bulun.</span><span class="sxs-lookup"><span data-stu-id="201cb-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="201cb-107">İki ad sunucusu kaydını şu değerlerle eşleşecek biçimde oluşturun veya düzenleyin:</span><span class="sxs-lookup"><span data-stu-id="201cb-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="201cb-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="201cb-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="201cb-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="201cb-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="201cb-110">Değişiklikleri kaydedin.</span><span class="sxs-lookup"><span data-stu-id="201cb-110">Save changes.</span></span>

<span data-ttu-id="201cb-111">Bu makalede de ayrıntılı yönergeler bulabilirsiniz: [Herhangi bir etki alanı kayıt şirketiyle Office 365’i ayarlamak için ad sunucularını değiştirme](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="201cb-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  