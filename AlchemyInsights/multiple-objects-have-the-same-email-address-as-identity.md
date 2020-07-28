---
title: Birden çok nesne kimlikle aynı e-posta adresine sahiptir
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439707"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="0954f-102">Birden çok nesne kimlikle aynı e-posta adresine sahiptir</span><span class="sxs-lookup"><span data-stu-id="0954f-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="0954f-103">**Birden çok nesne**</span><span class="sxs-lookup"><span data-stu-id="0954f-103">**Multiple objects**</span></span>

<span data-ttu-id="0954f-104">Bu hatanın yaygın nedenlerinden biri, kimlikle aynı e-posta adresine sahip birden çok nesnenin varlığında bir Outlook Web Access isteğini düzgün bir şekilde yönlendirememektir.</span><span class="sxs-lookup"><span data-stu-id="0954f-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="0954f-105">Bu nesneleri bulmak için aşağıdaki komutları çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="0954f-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="0954f-106">· Alıcı Al<email address></span><span class="sxs-lookup"><span data-stu-id="0954f-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="0954f-107">· Kullanıcı Al<email address></span><span class="sxs-lookup"><span data-stu-id="0954f-107">· Get-User <email address></span></span>

<span data-ttu-id="0954f-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="0954f-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="0954f-109">· İletişim Kurun<email address></span><span class="sxs-lookup"><span data-stu-id="0954f-109">· Get-Contact <email address></span></span>

<span data-ttu-id="0954f-110">· Posta Kutusu Al <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="0954f-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="0954f-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="0954f-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="0954f-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="0954f-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="0954f-113">Sorunu gidermek için, aynı e-posta kimliğine sahip birden çok nesneyi kaldırın ve belirli e-posta kimliğine sahip tek bir nesne olduğundan ve alıcı türünün UserMailbox olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="0954f-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="0954f-114">**Aynı adres iş ve tüketici posta kutuları için kullanılır**</span><span class="sxs-lookup"><span data-stu-id="0954f-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="0954f-115">Başka bir nedeni aynı adres iş ve tüketici posta kutuları için kullanılır.</span><span class="sxs-lookup"><span data-stu-id="0954f-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="0954f-116">Bu durumda, Cafe bu senaryoyu destekleyene kadar kullanıcının birincil tüketici takma adını değiştirmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="0954f-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="0954f-117">Bu müdahale olmadan gitmez kalıcı bir hatadır.</span><span class="sxs-lookup"><span data-stu-id="0954f-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="0954f-118">Ayrıntılar için Microsoft [hesabınızın e-posta adresini veya telefon numarasını değiştir'e](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)bakın.</span><span class="sxs-lookup"><span data-stu-id="0954f-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>