---
title: Outlook Masaüstü geri çağırma veya değiştirme bir e-posta iletisi
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389803"
---
# <a name="recall-or-replace-an-email-message"></a><span data-ttu-id="ac9c8-102">Çağrılacağı ya da bir e-posta iletisi</span><span class="sxs-lookup"><span data-stu-id="ac9c8-102">Recall or replace an email message</span></span>

- <span data-ttu-id="ac9c8-103">Yönetici, **PowerShell kullanan kullanıcılar adına ileti geri çekme**olabilir.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="ac9c8-104">Yönetim Merkezi iletilerden Çekemiyor.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="ac9c8-105">**Yalnızca kuruluşunuzdaki kişilere gönderilen iletileri geri çağırma**kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="ac9c8-106">Örneğin, Gmail adresine ileti gönderilmişse, onu Çekemiyor.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="ac9c8-107">**Yalnızca PC'de 2016 Outlook uygulamasından gönderilen iletileri geri çağırma**kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="ac9c8-108">Bir kullanıcı Mac için Outlook veya Outlook Web kullanarak bir ileti gönderirse, Çekemiyor.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="ac9c8-109">Çağrılacağı ya da bir e-posta iletisi için:</span><span class="sxs-lookup"><span data-stu-id="ac9c8-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="ac9c8-110">Gönderilmiş Öğeler klasörü Outlook penceresinin soldaki klasör bölmesinde seçin.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="ac9c8-111">Açmak için geri çekmek istediğiniz iletiyi çift tıklatın.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="ac9c8-112">**İleti** sekmesini seçin ve sonra **Eylemler**seçin > **Bu iletiyi Geri Çağır**.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="ac9c8-113">**Bu iletinin okunmamış kopyalarını sil** veya **Okunmamış kopyaları sil ve yerine yeni iletiler koy**seçin ve **Tamam**' ı seçin.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="ac9c8-114">Yeni ileti gönderiyorsanız, iletinizi oluşturun ve **Gönder**' i seçin.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="ac9c8-115">Başarı veya başarısızlık ileti geri çağırma alıcının Outlook ayarlarına bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="ac9c8-116">Geri çekme üzerinde denetlemek adımlar için [Bu makaleye](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)bakın.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="ac9c8-117">Arama ve kuruluşunuzdaki e-posta iletilerini silme</span><span class="sxs-lookup"><span data-stu-id="ac9c8-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="ac9c8-118">Genel Yönetici değilseniz, eBulma Yöneticisi rolü veya uyumluluk arama yönetimi rolü için iletileri aramak için hesabınıza eklenmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="ac9c8-119">İletileri silmek için Kuruluş Yönetimi rol grubunun ya da arama ve temizleme yönetim rolü katılmak gerekir.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="ac9c8-120">Bu roller için izinleri [Güvenlik ve Uyumluluk Merkezi](https://go.microsoft.com/fwlink/?linkid=2083731)atanır.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="ac9c8-121">İletiyi silmek için bulmak için [arama içerik oluşturma](https://docs.microsoft.com/office365/securitycompliance/content-search) .</span><span class="sxs-lookup"><span data-stu-id="ac9c8-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="ac9c8-122">[Güvenlik ve Uyumluluk Merkezi PowerShell bağlanın](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ac9c8-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="ac9c8-123">Çok faktörlü kimlik doğrulaması kullanıyorsanız, [çok faktörlü kimlik doğrulama kullanarak bağlan Office 365 güvenlik ve Uyumluluk Merkezi PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)bakın.</span><span class="sxs-lookup"><span data-stu-id="ac9c8-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>