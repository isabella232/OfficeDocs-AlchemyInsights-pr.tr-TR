---
title: Silinen posta kutusunu geri yükleme
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "360"
- "3500005"
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: 18e56305b60469422a154ffa1b097c238baaae16
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764676"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="42370-102">Silinen posta kutusunu geri yükleme</span><span class="sxs-lookup"><span data-stu-id="42370-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="42370-103">Bir kullanıcı Exchange Online lisansını kaybettiğinde, posta kutusu 30 gün boyunca saklanır ve yalnızca kullanıcıya lisansı yeniden atayarak kurtarılabilir.</span><span class="sxs-lookup"><span data-stu-id="42370-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="42370-104">*Bu sadece 30 gün içinde çalışacaktır.*</span><span class="sxs-lookup"><span data-stu-id="42370-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="42370-105">Microsoft 365 yönetici merkezinde, **Kullanıcılar** \> **Etkin kullanıcılar** sayfasına gidin.</span><span class="sxs-lookup"><span data-stu-id="42370-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="42370-106">Söz konusu kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="42370-106">Select the user in question.</span></span>

2. <span data-ttu-id="42370-107">**Lisanslar ve Uygulamalar** sekmesinde, Exchange Online lisansını atayın ve **değişiklikleri kaydet'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="42370-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="42370-108">Paylaşılan posta kutusunu kurtarmaya çalışıyorsanız, 30 gün boyunca kurtarılabilir.</span><span class="sxs-lookup"><span data-stu-id="42370-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="42370-109">**Bunları Kullanıcılar** \> **Silinen kullanıcılar**altında bulabilirsiniz; paylaşılan posta kutuları lisans gerektirmez.</span><span class="sxs-lookup"><span data-stu-id="42370-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="42370-110">Silinmiş bir kullanıcıyı geri yüklemeniz gerektiğini fark ederseniz, lütfen [bir kullanıcıyı geri yükle'ye](https://docs.microsoft.com/office365/admin/add-users/restore-user)bakın.</span><span class="sxs-lookup"><span data-stu-id="42370-110">If you realize that you need to restore a deleted user, please see [Restore a user](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span></span>
  