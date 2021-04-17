---
title: Ad Sunucularını Değiştirme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818632"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="6083c-102">Etki alanı ad sunucularınızı Microsoft’a işaret edecek şekilde güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="6083c-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="6083c-103">Not: Ad sunucusu değişikliklerinin yayılması bazen 48 saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="6083c-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="6083c-p101">Microsoft 365’te etki alanınızı ayarlamak için kayıt şirketinizdeki ad sunucularının güncelleştirilmesi gerekir. Etki alanı kayıt şirketinizde ad sunucusu kayıtlarınızı oluşturun veya düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="6083c-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="6083c-106">Etki alanı kayıt şirketinizin web sitesine gidin ve ad sunucularını düzenleyebileceğiniz alanı bulun.</span><span class="sxs-lookup"><span data-stu-id="6083c-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="6083c-107">İki ad sunucusu kaydını şu değerlerle eşleşecek biçimde oluşturun veya düzenleyin:</span><span class="sxs-lookup"><span data-stu-id="6083c-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="6083c-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="6083c-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="6083c-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="6083c-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="6083c-110">Değişiklikleri kaydedin.</span><span class="sxs-lookup"><span data-stu-id="6083c-110">Save changes.</span></span>

<span data-ttu-id="6083c-111">Bu makalede de ayrıntılı yönergeler bulabilirsiniz: [Herhangi bir etki alanı kayıt şirketiyle ad sunucularını değiştirme](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="6083c-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  