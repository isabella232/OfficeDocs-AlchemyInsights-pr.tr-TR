---
title: Arşiv posta kutusuna e-posta iletileri taşı
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 2147c70f64087bf95fc4e39c193caeac3b2c5361
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660403"
---
<span data-ttu-id="5c51a-p101">Arşivleme işlemi öğeleri arşiv posta sorunlarınız. Aşağıdaki adımları gerçekleştirdiğiniz emin olun:</span><span class="sxs-lookup"><span data-stu-id="5c51a-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="5c51a-p102">Bir **posta kutusu arşiv** etkinleştirilmiş olduğunu doğrulayın. Tersi durumda, arşiv posta kutusunu etkinleştirmek için [Bu makalede](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) adımları kullanın.</span><span class="sxs-lookup"><span data-stu-id="5c51a-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="5c51a-106">Exchange Yönetim Merkezi'ndeki **Uyumluluk Yönetimi**altında **Tutma etiketleri** seçin, **arşive Taşı** eylemini istenen **Bekletme yaş**içeren bir **bekletme etiketi** oluşturmak.</span><span class="sxs-lookup"><span data-stu-id="5c51a-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="5c51a-107">Exchange Yönetim Merkezi, **Bekletme ilkeleri**seçin, bir **Bekletme ilkesi** oluşturun ve **arşive Taşı** bekletme etiketinizi bu ilkeye eklemek.</span><span class="sxs-lookup"><span data-stu-id="5c51a-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="5c51a-p103">[Bekletme ilkesini atamak](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) için belirli bir kullanıcının posta kutusu. Hem **birincil** hem de **Arşiv** posta kutusu için aynı ilke uygulanacaktır.</span><span class="sxs-lookup"><span data-stu-id="5c51a-p103">[Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="5c51a-p104">Kullanıcının posta kutusu şimdi öğeleri arşiv posta kutusuna taşımak için bir Arşiv İlkesi olmalıdır. Yönetilen Klasör Yardımcısı (çalıştırmak ve kullanıcının posta kutusu için yeni ayarları uygulamak için MFA) zorlamak gerekli olabilir. Yönetilen Klasör Yardımcısı belirli bir posta kutusu için başlatmak için [EXO PowerShell için bağlı](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) çalışırken aşağıdaki komutu çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="5c51a-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="5c51a-113">Bir Arşiv İlkesi hakkında daha fazla bilgi istiyorsanız, [posta kutuları için bir arşiv ve silme ilkesini ayarlama](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="5c51a-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

