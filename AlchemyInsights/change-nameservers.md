---
title: Ad Sunucularını Değiştirme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706775"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="8b925-102">Etki alanı ad sunucularınızı Microsoft’a işaret edecek şekilde güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="8b925-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="8b925-103">Not: Ad sunucusu değişikliklerinin yayılması bazen 48 saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="8b925-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="8b925-p101">Microsoft 365’te etki alanınızı ayarlamak için kayıt şirketinizdeki ad sunucularının güncelleştirilmesi gerekir. Etki alanı kayıt şirketinizde ad sunucusu kayıtlarınızı oluşturun veya düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="8b925-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="8b925-106">Etki alanı kayıt şirketinizin web sitesine gidin ve ad sunucularını düzenleyebileceğiniz alanı bulun.</span><span class="sxs-lookup"><span data-stu-id="8b925-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="8b925-107">İki ad sunucusu kaydını şu değerlerle eşleşecek biçimde oluşturun veya düzenleyin:</span><span class="sxs-lookup"><span data-stu-id="8b925-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="8b925-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="8b925-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="8b925-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="8b925-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="8b925-110">Değişiklikleri kaydedin.</span><span class="sxs-lookup"><span data-stu-id="8b925-110">Save changes.</span></span>

<span data-ttu-id="8b925-111">Bu makalede de ayrıntılı yönergeler bulabilirsiniz: [Herhangi bir etki alanı kayıt şirketiyle ad sunucularını değiştirme](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="8b925-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  