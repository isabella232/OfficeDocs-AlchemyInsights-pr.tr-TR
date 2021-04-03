---
title: Silinmiş bir Microsoft 365 grubunu geri yükleme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505730"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="432d7-102">Silinmiş bir Microsoft 365 grubunu geri yükleme</span><span class="sxs-lookup"><span data-stu-id="432d7-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="432d7-103">Silinen Microsoft 365 grubunu veya Microsoft Teams'i silme işleminin ardından 30 gün içinde geri yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="432d7-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="432d7-104">Microsoft 365 yönetim merkezinde oturum açma ve silinen grupları ve ekiplerin listesini yapmak [için, Microsoft 365 yönetim merkezine gidin.](https://aka.ms/RestoreDeletedGroup)</span><span class="sxs-lookup"><span data-stu-id="432d7-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="432d7-105">**Not:** Kiracı yöneticisine veya gruplar yöneticisi rolüne atanan hesabı kullanarak oturum açın.</span><span class="sxs-lookup"><span data-stu-id="432d7-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="432d7-106">Geri yüklenecek silinmiş Microsoft 365 grubunu/Teams'i seçin ve Geri Yükle **grubuna tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="432d7-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="432d7-107">Çakışan bir SMTP adresi nedeniyle grup geri yüklenebilirse, çakışmaya neden olan nesneyi bulmak ve SMTP adresini kaldırmak için aşağıdaki komutu kullanın:</span><span class="sxs-lookup"><span data-stu-id="432d7-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="432d7-108">**Not:** Bazı durumlarda, grubun ve tüm verilerin geri yüklenebilir olması 24 saat kadar sürebilir.</span><span class="sxs-lookup"><span data-stu-id="432d7-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="432d7-109">Daha fazla bilgi edinmek veya PowerShell kullanarak grupları geri yükleme hakkında bilgi edinmek için, [bkz. Silinmiş Microsoft 365 grubunu](https://go.microsoft.com/fwlink/?linkid=867802)geri yükleme.</span><span class="sxs-lookup"><span data-stu-id="432d7-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>