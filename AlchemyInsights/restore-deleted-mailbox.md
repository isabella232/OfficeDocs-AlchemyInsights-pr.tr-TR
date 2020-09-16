---
title: Silinmiş posta kutusunu geri yükleme
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
ms.openlocfilehash: 899eb7e171d125c509871c219f99dfd1106b858a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728091"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="e517e-102">Silinmiş posta kutusunu geri yükleme</span><span class="sxs-lookup"><span data-stu-id="e517e-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="e517e-103">Kullanıcı Exchange Online lisansını kaybettiğinde, posta kutusu 30 gün boyunca korunur ve lisans yalnızca kullanıcıya yeniden atanarak kurtarılabilir.</span><span class="sxs-lookup"><span data-stu-id="e517e-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="e517e-104">*Bu, yalnızca 30 gün içinde çalışacaktır.*</span><span class="sxs-lookup"><span data-stu-id="e517e-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="e517e-105">Microsoft 365 Yönetim merkezinde, **Kullanıcılar** \> **etkin kullanıcılar** sayfasına gidin.</span><span class="sxs-lookup"><span data-stu-id="e517e-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="e517e-106">Söz konusu kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="e517e-106">Select the user in question.</span></span>

2. <span data-ttu-id="e517e-107">**Lisanslar ve uygulamalar** sekmesinde, Exchange Online lisansını atayın ve **Değişiklikleri Kaydet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="e517e-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="e517e-108">Paylaşılan bir posta kutusunu kurtarmaya çalışıyorsanız, bu, 30 gün boyunca kurtarılabilir.</span><span class="sxs-lookup"><span data-stu-id="e517e-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="e517e-109">**Kullanıcıları** \> **silinen kullanıcılar**altında bulabilirsiniz; paylaşılan posta kutuları lisans gerektirmez.</span><span class="sxs-lookup"><span data-stu-id="e517e-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="e517e-110">Silinmiş bir kullanıcıyı geri yüklemeniz gerektiğini fark ederseniz, lütfen [kullanıcıyı geri yükleme](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)bölümüne bakın.</span><span class="sxs-lookup"><span data-stu-id="e517e-110">If you realize that you need to restore a deleted user, please see [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
  