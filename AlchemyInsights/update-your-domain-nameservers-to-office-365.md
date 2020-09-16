---
title: Etki alanı ad sunucularınızı Microsoft’a işaret edecek şekilde güncelleştirme
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734931"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="4dfcb-102">Etki alanı ad sunucularınızı Microsoft’a işaret edecek şekilde güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="4dfcb-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="4dfcb-103">Not: Ad sunucusu değişikliklerinin yayılması bazen 48 saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="4dfcb-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="4dfcb-104">Etki alanınızı Microsoft ile ayarlamak için, kayıt şirketinizde ad sunucularının güncellenmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="4dfcb-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="4dfcb-105">Etki alanı kayıt şirketinizde ad sunucusu kayıtlarınızı oluşturun veya düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="4dfcb-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="4dfcb-106">Etki alanı kayıt şirketinizin web sitesine gidin ve ad sunucularını düzenleyebileceğiniz alanı bulun.</span><span class="sxs-lookup"><span data-stu-id="4dfcb-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="4dfcb-107">İki ad sunucusu kaydını şu değerlerle eşleşecek biçimde oluşturun veya düzenleyin:</span><span class="sxs-lookup"><span data-stu-id="4dfcb-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="4dfcb-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4dfcb-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="4dfcb-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4dfcb-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="4dfcb-110">Değişiklikleri kaydedin.</span><span class="sxs-lookup"><span data-stu-id="4dfcb-110">Save changes.</span></span>

<span data-ttu-id="4dfcb-111">Bu makalede ayrıntılı yönergeleri de bulabilirsiniz: [ad sunucularını değiştirme Microsoft 365 'yi etki alanı kaydediciyle ayarlamak için](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="4dfcb-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  