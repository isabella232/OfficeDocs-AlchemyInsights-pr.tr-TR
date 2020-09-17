---
title: E-posta iletisini geri çekme veya değiştirme
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 2e711679e7db7293d9e7e6f68d0662f03047c23d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799224"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="2beb2-102">Microsoft 365 'de e-posta iletisini geri çekme veya değiştirme</span><span class="sxs-lookup"><span data-stu-id="2beb2-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="2beb2-103">**Yalnızca kuruluşunuzdaki kişilere gönderilen iletileri geri**yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="2beb2-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="2beb2-104">Örneğin, ileti gmail adresine gönderildiyse, geri çekilemiyor.</span><span class="sxs-lookup"><span data-stu-id="2beb2-104">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="2beb2-105">**PC Için Outlook 2016 ' den gönderilen iletileri geri çekmeniz**yeterlidir.</span><span class="sxs-lookup"><span data-stu-id="2beb2-105">You can **only recall messages sent from Outlook 2016 for the PC**.</span></span> <span data-ttu-id="2beb2-106">Bir Kullanıcı, Mac için Outlook veya Web üzerinde Outlook kullanan bir ileti gönderirse, geri çekemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="2beb2-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="2beb2-107">Yöneticiyseniz, **PowerShell kullanarak iletileri Kullanıcı adına geri çekbırakabilirsiniz**.</span><span class="sxs-lookup"><span data-stu-id="2beb2-107">If you're an admin, you can **recall messages on behalf of users by using PowerShell**.</span></span> <span data-ttu-id="2beb2-108">Yönetim merkezinden iletileri geri çekemezsiniz.</span><span class="sxs-lookup"><span data-stu-id="2beb2-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="2beb2-109">Daha fazla bilgi için "kuruluşunuzdaki e-posta iletilerini arayın ve silin" için aşağı kaydırın.</span><span class="sxs-lookup"><span data-stu-id="2beb2-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="2beb2-110">**Gönderdiğiniz e-posta iletisini geri çekme veya değiştirme**</span><span class="sxs-lookup"><span data-stu-id="2beb2-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="2beb2-111">Outlook penceresinin solundaki klasör bölmesinde Gönderilmiş Öğeler klasörünü seçin.</span><span class="sxs-lookup"><span data-stu-id="2beb2-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="2beb2-112">Geri çekmek istediğiniz iletiyi açın.</span><span class="sxs-lookup"><span data-stu-id="2beb2-112">Open the message that you want to recall.</span></span> <span data-ttu-id="2beb2-113">İletiyi açmak için çift tıklatın.</span><span class="sxs-lookup"><span data-stu-id="2beb2-113">You must double-click to open the message.</span></span> <span data-ttu-id="2beb2-114">İletiyi, okuma bölmesinde görünecek şekilde seçmek iletiyi geri çekmenizi sağlar.</span><span class="sxs-lookup"><span data-stu-id="2beb2-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="2beb2-115">İleti sekmesinden, **Actions**  >  **Bu iletiyi geri çek**eylemler 'i seçin.</span><span class="sxs-lookup"><span data-stu-id="2beb2-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="2beb2-116">**Bu iletinin okunmamış kopyalarını sil** 'i veya **Okunmamış kopyaları sil 'i seçin ve yeni bir iletiyle değiştirin**, ardından **Tamam 'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="2beb2-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="2beb2-117">Değiştirme iletisi gönderiyorsanız iletiyi oluşturun ve **Gönder**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="2beb2-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="2beb2-118">İletinin geri çekme başarısı veya başarısızlığı, alıcıların Outlook 'taki ayarlarına bağlıdır.</span><span class="sxs-lookup"><span data-stu-id="2beb2-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="2beb2-119">Geri çekmeyi denetleme dahil olmak üzere daha fazla bilgi için, [gönderdiğiniz e-posta Iletisini geri çekme veya değiştirme](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="2beb2-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="2beb2-120">***Kuruluşunuzdaki e-posta Iletilerini arama ve silme*** Kuruluşunuzdaki e-posta iletilerini aramak ve silmek için, genel bir yönetici olmanız en kolay yoldur. Genel yönetici değilseniz, hesabınız eBulma Yöneticisi rol grubuna veya uyumluluk arama yönetimi rolüne eklenmelidir.</span><span class="sxs-lookup"><span data-stu-id="2beb2-120">***Search for and delete email messages in your organization*** To search for and delete email messages in your organization, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="2beb2-121">İletileri silmek için, Kuruluş Yönetimi rol grubuna veya arama ve Temizleme Yönetim rolüne katılmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="2beb2-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="2beb2-122">Bu rollerin izinleri [güvenlik & Uyumluluk Merkezi](https://protection.office.com/)'nde atanır.</span><span class="sxs-lookup"><span data-stu-id="2beb2-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="2beb2-123">Silinecek iletiyi bulmak için [içerik araması oluşturun](https://docs.microsoft.com/microsoft-365/compliance/content-search) .</span><span class="sxs-lookup"><span data-stu-id="2beb2-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="2beb2-124">[Güvenlik & Uyumluluk Merkezi PowerShell 'e bağlanın](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="2beb2-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span> 

<span data-ttu-id="2beb2-125">MFA kullanıyorsanız, [Multi-Factor Authentication kullanarak Microsoft 365 güvenlik & Uyumluluk Merkezi PowerShell 'e bağlanın](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="2beb2-125">If you're using MFA, see [Connect to Microsoft 365 security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span> 
