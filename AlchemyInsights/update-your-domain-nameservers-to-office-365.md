---
title: Etki alanı ad sunucularınızı Office 365'e güncelleştirme
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742208"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="4ccbb-102">Etki alanı ad sunucularınızı Office 365'e güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="4ccbb-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="4ccbb-103">Not: Ad sunucusu değişikliklerinin yayılması bazen 48 saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="4ccbb-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="4ccbb-p101">Office 365’te etki alanınızı ayarlamak için kayıt şirketinizdeki ad sunucularının güncelleştirilmesi gerekir. Etki alanı kayıt şirketinizde ad sunucusu kayıtlarınızı oluşturun veya düzenleyin.</span><span class="sxs-lookup"><span data-stu-id="4ccbb-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="4ccbb-106">Etki alanı kayıt şirketinizin web sitesine gidin ve ad sunucularını düzenleyebileceğiniz alanı bulun.</span><span class="sxs-lookup"><span data-stu-id="4ccbb-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="4ccbb-107">İki ad sunucusu kaydını şu değerlerle eşleşecek biçimde oluşturun veya düzenleyin:</span><span class="sxs-lookup"><span data-stu-id="4ccbb-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="4ccbb-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4ccbb-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="4ccbb-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4ccbb-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="4ccbb-110">Değişiklikleri kaydedin.</span><span class="sxs-lookup"><span data-stu-id="4ccbb-110">Save changes.</span></span>

<span data-ttu-id="4ccbb-111">Bu makalede de ayrıntılı yönergeler bulabilirsiniz: [Herhangi bir etki alanı kayıt şirketiyle Office 365’i ayarlamak için ad sunucularını değiştirme](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="4ccbb-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  