---
title: Geri yükleme silinmiş posta kutusu
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
ms.openlocfilehash: 44b23be5e75a0669821bbeb07b0f064eeef6d021
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666392"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="d4d22-102">Silinen bir posta kutusunu geri yükleme</span><span class="sxs-lookup"><span data-stu-id="d4d22-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="d4d22-103">Bir kullanıcı bir Exchange Online lisans kaybettiğinde, kendi posta kutusu 30 gün süreyle korunur ve yalnızca lisans kullanıcıya yeniden atayarak kurtarıldı.</span><span class="sxs-lookup"><span data-stu-id="d4d22-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="d4d22-104">*Bu 30 gün içinde çalışır.*</span><span class="sxs-lookup"><span data-stu-id="d4d22-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="d4d22-105">**Kullanıcıların** Microsoft 365 Yönetim Merkezi'nde Git \> **Etkin kullanıcılar** sayfa.</span><span class="sxs-lookup"><span data-stu-id="d4d22-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="d4d22-106">Söz konusu kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="d4d22-106">Select the user in question.</span></span>

2. <span data-ttu-id="d4d22-107">**Lisanslar ve uygulamalar** sekmesinde, Exchange Online lisans atayın ve **Değişiklikleri Kaydet**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="d4d22-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="d4d22-108">Paylaşılan bir posta kutusunu kurtarmak çalışıyorsanız, bunun da 30 gün boyunca kurtarılabilir.</span><span class="sxs-lookup"><span data-stu-id="d4d22-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="d4d22-109">**Kullanıcılar** altında bulabilirsiniz \> **Silinen kullanıcıların**; Paylaşılan posta kutuları için lisans gerekmez.</span><span class="sxs-lookup"><span data-stu-id="d4d22-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="d4d22-110">Silinmiş bir kullanıcı geri gerektiğini fark ederseniz, [bir kullanıcının Office 365'te geri](https://docs.microsoft.com/office365/admin/add-users/restore-user)bakın.</span><span class="sxs-lookup"><span data-stu-id="d4d22-110">If you realize that you need to restore a deleted user, please see [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span></span>
  