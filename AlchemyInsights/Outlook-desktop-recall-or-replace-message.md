---
title: Outlook masaüstü bir e-posta iletisini geri çekme veya değiştirme
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664010"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="13e06-102">Outlook e-posta iletisini geri çekme veya değiştirme</span><span class="sxs-lookup"><span data-stu-id="13e06-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="13e06-103">Yönetici olarak, **PowerShell kullanarak kullanıcıları adına iletileri geri çekbırakabilirsiniz**.</span><span class="sxs-lookup"><span data-stu-id="13e06-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="13e06-104">Yönetim merkezinden iletileri geri çekemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="13e06-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="13e06-105">**Yalnızca kuruluşunuzdaki kişilere gönderilen iletileri geri**yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="13e06-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="13e06-106">Örneğin, ileti gmail adresine gönderildiyse, geri çekilemiyor.</span><span class="sxs-lookup"><span data-stu-id="13e06-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="13e06-107">**Bilgisayarda yalnızca Outlook 2016 tarafından gönderilen iletileri geri çekmeniz**yeterlidir.</span><span class="sxs-lookup"><span data-stu-id="13e06-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="13e06-108">Bir Kullanıcı, Mac için Outlook veya Web üzerinde Outlook kullanan bir ileti gönderirse, geri çekemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="13e06-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="13e06-109">E-posta iletisini geri çekmek veya değiştirmek için:</span><span class="sxs-lookup"><span data-stu-id="13e06-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="13e06-110">Outlook penceresinin solundaki klasör bölmesinde Gönderilmiş Öğeler klasörünü seçin.</span><span class="sxs-lookup"><span data-stu-id="13e06-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="13e06-111">Geri çekmek istediğiniz iletiye çift tıklayarak açın.</span><span class="sxs-lookup"><span data-stu-id="13e06-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="13e06-112">**İleti** sekmesini ve sonra da eylemler 'i seçin **Actions**  >  **Recall This Message**.</span><span class="sxs-lookup"><span data-stu-id="13e06-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="13e06-113">**Bu iletinin okunmamış kopyalarını sil** 'i veya **Okunmamış kopyaları sil**'i seçin ve sonra da **Tamam 'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="13e06-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="13e06-114">Değiştirme iletisi gönderiyorsanız iletiyi oluşturun ve **Gönder**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="13e06-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="13e06-115">İletinin geri çekme başarısı veya başarısızlığı, alıcının Outlook 'taki ayarlarına bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="13e06-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="13e06-116">Geri çekmeyi denetleme adımları için [Bu makaleye](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)bakın.</span><span class="sxs-lookup"><span data-stu-id="13e06-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="13e06-117">Kuruluşunuzdaki e-posta iletilerini arama ve silme</span><span class="sxs-lookup"><span data-stu-id="13e06-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="13e06-118">Genel yönetici değilseniz, hesap aramak için hesabınızın eBulma Yöneticisi rolüne veya uyumluluk arama yönetimi rolüne eklenmesi gerekir.</span><span class="sxs-lookup"><span data-stu-id="13e06-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="13e06-119">İletileri silmek için, Kuruluş Yönetimi rol grubuna veya arama ve Temizleme Yönetim rolüne katılmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="13e06-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="13e06-120">Bu rollerin izinleri [güvenlik ve Uyumluluk Merkezi](https://go.microsoft.com/fwlink/?linkid=2083731)'nde atanır.</span><span class="sxs-lookup"><span data-stu-id="13e06-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="13e06-121">Silinecek iletiyi bulmak için [içerik araması oluşturun](https://docs.microsoft.com/microsoft-365/compliance/content-search) .</span><span class="sxs-lookup"><span data-stu-id="13e06-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="13e06-122">[Güvenlik ve Uyumluluk Merkezi PowerShell 'e bağlanın](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="13e06-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="13e06-123">Multi-Factor Authentication kullanıyorsanız, [Multi-Factor Authentication kullanarak Microsoft 365 güvenlik ve Uyumluluk Merkezi PowerShell 'e bağlanın](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="13e06-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>