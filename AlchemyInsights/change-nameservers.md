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
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736669"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="4df89-102">Etki alanı ad sunucularınızı Office 365'e güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="4df89-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="4df89-103">Not: Ad sunucusu değişikliklerinin yayılması bazen 48 saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="4df89-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="4df89-p101">Office 365’te etki alanınızı ayarlamak için kayıt şirketinizdeki ad sunucularının güncelleştirilmesi gerekir. Etki alanı kayıt şirketinizde ad sunucusu kayıtlarınızı oluşturun veya düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="4df89-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="4df89-106">Etki alanı kayıt şirketinizin web sitesine gidin ve ad sunucularını düzenleyebileceğiniz alanı bulun.</span><span class="sxs-lookup"><span data-stu-id="4df89-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="4df89-107">İki ad sunucusu kaydını şu değerlerle eşleşecek biçimde oluşturun veya düzenleyin:</span><span class="sxs-lookup"><span data-stu-id="4df89-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="4df89-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4df89-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="4df89-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4df89-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="4df89-110">Değişiklikleri kaydedin.</span><span class="sxs-lookup"><span data-stu-id="4df89-110">Save changes.</span></span>

<span data-ttu-id="4df89-111">Bu makalede de ayrıntılı yönergeler bulabilirsiniz: [Herhangi bir etki alanı kayıt şirketiyle Office 365’i ayarlamak için ad sunucularını değiştirme](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="4df89-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  