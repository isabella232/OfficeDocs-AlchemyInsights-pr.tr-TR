---
title: Posta kutusu için otomatik yanıtları ayarlama
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820954"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="95791-102">Kullanıcının posta kutusu için otomatik yanıtları ayarlama</span><span class="sxs-lookup"><span data-stu-id="95791-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="95791-103">**1. Yöntem**</span><span class="sxs-lookup"><span data-stu-id="95791-103">**Method 1**</span></span>

1. <span data-ttu-id="95791-104">Microsoft 365 portalında oturum açın.</span><span class="sxs-lookup"><span data-stu-id="95791-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="95791-105">**Kullanıcılar > Etkin kullanıcılar**’a (veya paylaşılan posta kutusunda ayarlıyorsanız **Gruplar > Paylaşılan posta kutuları**’na) gidin.</span><span class="sxs-lookup"><span data-stu-id="95791-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="95791-106">Microsoft Exchange posta kutusu olan bir kullanıcı seçin.</span><span class="sxs-lookup"><span data-stu-id="95791-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="95791-107">Sağ taraftaki açılır menüde **Posta ayarları > Otomatik yanıtlar**’a gidin (paylaşılan posta kutusu söz konusuysa açılır menüde doğrudan **Otomatik yanıtlar**’a tıklayın).</span><span class="sxs-lookup"><span data-stu-id="95791-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="95791-108">**2. Yöntem**</span><span class="sxs-lookup"><span data-stu-id="95791-108">**Method 2**</span></span>

1. <span data-ttu-id="95791-109">Yönetici kimlik bilgilerini kullanarak Microsoft 365 yönetim portalında oturum açın.</span><span class="sxs-lookup"><span data-stu-id="95791-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="95791-110">**Yönetim Merkezleri**’ni genişletin ve sonra **Exchange**’e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="95791-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="95791-111">Sağ üst köşedeki resme tıklayın, **Başka Kullanıcı**’ya tıklayın ve değiştirmek istediğiniz kullanıcı posta kutusunu seçin.</span><span class="sxs-lookup"><span data-stu-id="95791-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="95791-112">Sol tarafta **Seçenekler**’i seçin, **E-postayı Düzenle**’ye ve sonra da **Otomatik yanıtlar**’a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="95791-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="95791-113">**3. Yöntem**</span><span class="sxs-lookup"><span data-stu-id="95791-113">**Method 3**</span></span>

<span data-ttu-id="95791-114">Exchange Online PowerShell’de şu cmdlet’i çalıştırın:</span><span class="sxs-lookup"><span data-stu-id="95791-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="95791-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="95791-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="95791-116">Bu cmdlet hakkında daha fazla bilgi için bkz. [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="95791-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
