---
title: Outlook Desktop bir e-posta iletisi geri çağırma veya değiştirme
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36496131"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="33064-102">Outlook e-posta iletisi geri çağırma veya değiştirme</span><span class="sxs-lookup"><span data-stu-id="33064-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="33064-103">Yönetici olarak **PowerShell kullanan kullanıcılar adına iletileri geri çağırabilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="33064-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="33064-104">Yönetici merkezinden gelen iletileri geri çağıramazsınız.</span><span class="sxs-lookup"><span data-stu-id="33064-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="33064-105">Yalnızca **kuruluşunuzdaki kişilere gönderilen iletileri geri çağırabilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="33064-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="33064-106">İleti bir Gmail adresine gönderildiyse, örneğin, iletiyi geri çağıramazsınız.</span><span class="sxs-lookup"><span data-stu-id="33064-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="33064-107">Yalnızca **Outlook 2016'dan gönderilen iletileri pc'de hatırlayabilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="33064-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="33064-108">Bir kullanıcı web'de Mac için Outlook veya Outlook kullanarak bir ileti gönderirse, bunu geri çağıramazsınız.</span><span class="sxs-lookup"><span data-stu-id="33064-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="33064-109">Bir e-posta iletisini geri çağırmak veya değiştirmek için:</span><span class="sxs-lookup"><span data-stu-id="33064-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="33064-110">Outlook penceresinin solundaki klasör bölmesinde Gönderilmiş Öğeler klasörünü seçin.</span><span class="sxs-lookup"><span data-stu-id="33064-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="33064-111">Açmak için hatırlamak istediğiniz iletiyi çift tıklatın.</span><span class="sxs-lookup"><span data-stu-id="33064-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="33064-112">**İleti** sekmesini seçin ve ardından **Eylemler** > **Bu İletiyi Geri Çağır'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="33064-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="33064-113">**Bu iletinin okunmamış kopyalarını sil'i** seçin veya **okunmamış kopyaları silin ve yeni bir iletiyle değiştirin**ve ardından **Tamam'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="33064-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="33064-114">Yeni bir ileti gönderiyorsanız, iletiyi oluşturun ve sonra **Gönder'i**seçin.</span><span class="sxs-lookup"><span data-stu-id="33064-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="33064-115">İleti geri çağırmanın başarısı veya başarısızlığı, alıcının Outlook'taki ayarlarına bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="33064-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="33064-116">Geri çağırmayı denetlemek için adımlar için [bu makaleye](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)bakın.</span><span class="sxs-lookup"><span data-stu-id="33064-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="33064-117">Kuruluşunuzdaki e-posta iletilerini arama ve silme</span><span class="sxs-lookup"><span data-stu-id="33064-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="33064-118">Genel bir yönetici değilseniz, iletileri aramak için hesabınızın eDiscovery Manager rolüne veya Uyumluluk Arama yönetimi rolüne eklenmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="33064-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="33064-119">İletileri silmek için, Organizasyon Yönetimi rol grubuna veya Arama ve Temizleme yönetimi rolüne katılmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="33064-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="33064-120">Bu rolleriçin izinler [Güvenlik ve uyumluluk merkezinde](https://go.microsoft.com/fwlink/?linkid=2083731)atanır.</span><span class="sxs-lookup"><span data-stu-id="33064-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="33064-121">Silmek için ileti bulmak için [bir içerik araması oluşturun.](https://docs.microsoft.com/office365/securitycompliance/content-search)</span><span class="sxs-lookup"><span data-stu-id="33064-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="33064-122">[Güvenlik ve Uyumluluk Merkezi PowerShell'e bağlanın.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="33064-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="33064-123">Çok faktörlü kimlik doğrulama kullanıyorsanız, [çok faktörlü kimlik doğrulaması kullanarak Office 365 Güvenlik ve Uyumluluk Merkezi PowerShell'e bağlan'a](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)bakın.</span><span class="sxs-lookup"><span data-stu-id="33064-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>