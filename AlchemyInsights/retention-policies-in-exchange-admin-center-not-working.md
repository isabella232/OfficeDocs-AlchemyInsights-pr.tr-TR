---
title: Exchange Yönetici Merkezi'nde Bekletme İlkeleri çalışmıyor
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522827"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="9628c-102">Exchange Yönetici Merkezinde Bekletme İlkeleri</span><span class="sxs-lookup"><span data-stu-id="9628c-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="9628c-103">Aşağıda belirtilen ayarlar için otomatik denetimler yapmamızı istiyorsanız, bu sayfanın üst kısmındaki < arka düğmesini seçin ve ardından bekletme ilkeleriyle ilgili sorunları olan kullanıcının e-posta adresini girin.</span><span class="sxs-lookup"><span data-stu-id="9628c-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="9628c-104">**Sorun:** Exchange Yönetici Merkezi'nde yeni oluşturulan veya güncelleştirilen bekletme ilkeleri posta kutularına uygulanmaz veya öğeler arşiv posta kutusuna taşınmaz veya silinmez.</span><span class="sxs-lookup"><span data-stu-id="9628c-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="9628c-105">**Kök Nedenleri:**</span><span class="sxs-lookup"><span data-stu-id="9628c-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="9628c-106">Bunun **nedeni, Yönetilen Klasör Yardımcısı'nın** kullanıcının posta kutusunu işlememiş olması olabilir.</span><span class="sxs-lookup"><span data-stu-id="9628c-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="9628c-107">Yönetilen Klasör Yardımcısı, bulut tabanlı kuruluşunuzdaki her posta kutusunu yedi günde bir işlemeye çalışır.</span><span class="sxs-lookup"><span data-stu-id="9628c-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="9628c-108">Bekletme etiketini değiştirir veya bir posta kutusuna farklı bir bekletme ilkesi uygularsanız, Yönetilen Klasör Yardımcısı'nın posta kutusunu işlemesini bekleyebilir veya belirli bir posta kutusunu işlemek için Yönetilen Klasör Yardımcısı'nı başlatmak için Başlat Yönetilen Klasör Yardımcısı cmdlet'ini çalıştırabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="9628c-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="9628c-109">Bu cmdlet'i çalıştırmak, bekletme ilkesi veya bekletme etiketi ayarlarını sınamak veya sorun gidermek için yararlıdır.</span><span class="sxs-lookup"><span data-stu-id="9628c-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="9628c-110">Daha fazla bilgi için Yönetilen Klasör Yardımcısını Çalıştır'ı ziyaret [edin.](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)</span><span class="sxs-lookup"><span data-stu-id="9628c-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="9628c-111">**Çözüm:** Belirli bir posta kutusu için Yönetilen Klasör Yardımcısı'nı başlatmak için aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="9628c-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="9628c-112">**Bu,** posta kutusunda Beklet **etkinleştirilmişse** de oluşabilir.</span><span class="sxs-lookup"><span data-stu-id="9628c-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="9628c-113">Posta kutusu Bekletme Ambarı'na yerleştirilmişse, posta kutusundaki bekletme ilkesi bu süre içinde işleme alınmaz.</span><span class="sxs-lookup"><span data-stu-id="9628c-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="9628c-114">Bekletme ayarında daha fazla bilgilendirme için bkz: [Posta Kutusu Bekletme .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="9628c-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="9628c-115">**Çözüm:**</span><span class="sxs-lookup"><span data-stu-id="9628c-115">**Solution:**</span></span>
    
  - <span data-ttu-id="9628c-116">[EXO powershell'deki](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)belirli posta kutusundaki Bekletme Ayarı'nın durumunu denetleyin:</span><span class="sxs-lookup"><span data-stu-id="9628c-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="9628c-117">Belirli bir posta kutusunda Beklet'i **devre dışı kıtırmak** için aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="9628c-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="9628c-118">Şimdi, Yönetilen klasör Yardımcısı yeniden çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="9628c-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="9628c-119">**Not:** Bir posta kutusu 10 MB'dan küçükse, Yönetilen Klasör Yardımcısı posta kutusunu otomatik olarak işlemez.</span><span class="sxs-lookup"><span data-stu-id="9628c-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="9628c-120">Exchange Yönetici Merkezi'ndeki bekletme ilkeleri hakkında daha fazla bilgi için bkz:</span><span class="sxs-lookup"><span data-stu-id="9628c-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="9628c-121">Bekletme etiketleri ve bekletme ilkeleri</span><span class="sxs-lookup"><span data-stu-id="9628c-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="9628c-122">Posta kutularına bekletme ilkesi uygulama</span><span class="sxs-lookup"><span data-stu-id="9628c-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="9628c-123">Bekletme etiketleri ekleme veya kaldırma</span><span class="sxs-lookup"><span data-stu-id="9628c-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="9628c-124">Posta kutusuna yerleştirilen bekleme türünü belirleme</span><span class="sxs-lookup"><span data-stu-id="9628c-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
