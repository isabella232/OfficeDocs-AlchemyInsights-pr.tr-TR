---
title: Kuruluşun genel adres listesini ve çevrimdışı adres defterini yönetme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022669"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="c0ea5-102">Kuruluşun genel adres listesini (GAL) ve çevrimdışı adres defterini (OAB) yönetme</span><span class="sxs-lookup"><span data-stu-id="c0ea5-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="c0ea5-103">Genel adres listesi (GAL) kuruluşta posta özellikli nesnelerin (e-posta alabilen her tür alıcı) listesidir.</span><span class="sxs-lookup"><span data-stu-id="c0ea5-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="c0ea5-104">Her kuruluşta bir GAL otomatik olarak oluşturulur.</span><span class="sxs-lookup"><span data-stu-id="c0ea5-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="c0ea5-105">Kullanıcıları kuruluşa veya konuma göre ayırmak için ek GAL’ler oluşturabilirsiniz ama bir kullanıcı aynı anda tek bir GAL görebilir ve kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="c0ea5-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="c0ea5-106">Windows için Outlook gibi bazı e-posta istemcileri GAL’yi çevrimdışı kullanım için indirir.</span><span class="sxs-lookup"><span data-stu-id="c0ea5-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="c0ea5-107">Bu, çevrimdışı adres defteri (OAB) olarak bilinir.</span><span class="sxs-lookup"><span data-stu-id="c0ea5-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="c0ea5-108">Exchange Online’da OAB ancak 8 saatte bir güncelleştirilir ve bundan sonra istemcilerin yerel OAB kopyalarını güncelleştirmek için OAB’yi indirmeleri gerekir.</span><span class="sxs-lookup"><span data-stu-id="c0ea5-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="c0ea5-109">Tüm alıcı değişikliklerinin OAB’ye geçmeden önce GAL’de görünür olması gerekir.</span><span class="sxs-lookup"><span data-stu-id="c0ea5-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="c0ea5-110">Aşağıda yaygın kullanılan bazı GAL ve OAB yordamları verilmiştir:</span><span class="sxs-lookup"><span data-stu-id="c0ea5-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="c0ea5-111">Çeşitli nedenlerle bazı nesnelerin GAL’de gizlenmesini isteyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c0ea5-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="c0ea5-112">Bkz. [Alıcıları adres listesinde gizleme](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="c0ea5-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="c0ea5-113">Belirli kullanıcı gruplarına kuruluşun GAL’sinin özelleştirilmiş görünümlerini vermeniz gerekirse bkz. [Exchange Online’da adres defteri ilkeleri](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="c0ea5-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="c0ea5-114">[Exchange Online’da genel adres listesi oluşturun](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) ve GAL izinleriyle çalışmayı öğrenmek için [Exchange Online’da adres listeleri](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists) konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="c0ea5-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="c0ea5-115">Yeni GAL’ler oluşturursanız, yeni bir OAB de oluşturmak isteyebileceğinizi aklınızda bulundurun.</span><span class="sxs-lookup"><span data-stu-id="c0ea5-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="c0ea5-116">Bkz. [Çevrimdışı adres defteri yordamları](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="c0ea5-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
