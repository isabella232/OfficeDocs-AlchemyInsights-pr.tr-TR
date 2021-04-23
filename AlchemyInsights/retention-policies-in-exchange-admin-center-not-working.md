---
title: Exchange Yönetim Merkezi'nde Bekletme İlkeleri çalışmıyor
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952248"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="cfcd8-102">Exchange Yönetim Merkezi'nde Bekletme İlkeleri</span><span class="sxs-lookup"><span data-stu-id="cfcd8-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="cfcd8-103">Aşağıda adı geçen ayarlar için otomatik denetimleri çalıştırmamızı istemiyorsanız, bu sayfanın en üstünde yer alan geri düğmesini < seçin ve ardından bekletme ilkeleriyle ilgili sorunları olan kullanıcının e-posta adresini girin.</span><span class="sxs-lookup"><span data-stu-id="cfcd8-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="cfcd8-104">Exchange Yönetim Merkezi'nde bekletme ilkeleri posta kutularına veya arşiv posta kutusuna taşınmıyor olan öğelere uygulanmıyorsa, bekletme ilkeleriyle ilgili sorunlarınız varsa, şunları kontrol edin:</span><span class="sxs-lookup"><span data-stu-id="cfcd8-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="cfcd8-105">**Kök Nedenler:**</span><span class="sxs-lookup"><span data-stu-id="cfcd8-105">**Root Causes:**</span></span>

- <span data-ttu-id="cfcd8-106">**Yönetilen Klasör Yardımcısı** kullanıcının posta kutusunu işlemedi.</span><span class="sxs-lookup"><span data-stu-id="cfcd8-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="cfcd8-107">Yönetilen Klasör Yardımcısı, bulut tabanlı kuruluşta her posta kutusunu yedi günde bir işlemeyi çalışır.</span><span class="sxs-lookup"><span data-stu-id="cfcd8-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="cfcd8-108">**Çözüm:** Yönetilen Klasör Yardımcısı'nın çalıştırın.</span><span class="sxs-lookup"><span data-stu-id="cfcd8-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="cfcd8-109">**Posta kutusunda RetentionHold** **etkinleştirildi.**</span><span class="sxs-lookup"><span data-stu-id="cfcd8-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="cfcd8-110">Posta kutusu bir RetentionHold'a yerleştirilmişse, posta kutusunda bekletme ilkesi bu süre boyunca işlenmez.</span><span class="sxs-lookup"><span data-stu-id="cfcd8-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="cfcd8-111">**Çözüm:** Bekletme Bekletme ayarının durumunu denetleme ve gerektiğinde güncelleştirme.</span><span class="sxs-lookup"><span data-stu-id="cfcd8-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="cfcd8-112">Ayrıntılar için bkz. Posta [Kutusu Bekletme.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="cfcd8-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="cfcd8-113">**Not:** Posta kutusu 10 MB'den küçükse, Yönetilen Klasör Yardımcısı posta kutusunu otomatik olarak işlemez.</span><span class="sxs-lookup"><span data-stu-id="cfcd8-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="cfcd8-114">Exchange Yönetim Merkezi'nde bekletme ilkeleri hakkında daha fazla bilgi için bkz:</span><span class="sxs-lookup"><span data-stu-id="cfcd8-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="cfcd8-115">Bekletme etiketleri ve bekletme ilkeleri</span><span class="sxs-lookup"><span data-stu-id="cfcd8-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="cfcd8-116">[Posta kutularına bekletme ilkesi uygulama veya](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) Bekletme etiketleri ekleme veya [kaldırma](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="cfcd8-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="cfcd8-117">Posta kutusuna yerleştirilen tutma türünü belirleme</span><span class="sxs-lookup"><span data-stu-id="cfcd8-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
