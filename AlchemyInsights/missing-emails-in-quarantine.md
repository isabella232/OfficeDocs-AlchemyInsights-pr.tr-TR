---
title: Karantinada eksik e-postalar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569563"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="22223-102">Karantinada eksik e-postalar"</span><span class="sxs-lookup"><span data-stu-id="22223-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="22223-103">Yöneticiler [bu iletileri görüntüleyebilir, yayınlayabilir veya silebilir.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="22223-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="22223-104">Güvenlik & Uyumluluk Merkezi'ni açmak [https://protection.office.com](https://protection.office.com/) için.</span><span class="sxs-lookup"><span data-stu-id="22223-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="22223-105">Karantina sayfasını doğrudan açmak [https://protection.office.com/quarantine](https://protection.office.com/quarantine) için.</span><span class="sxs-lookup"><span data-stu-id="22223-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="22223-106">Aşağıdaki değerlere göre arama yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="22223-106">You can search by the following values:</span></span>  

- <span data-ttu-id="22223-107">**İleti Kimliği**: İletinin genel olarak benzersiz tanımlayıcısı.</span><span class="sxs-lookup"><span data-stu-id="22223-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="22223-108">Listede bir ileti seçerseniz, **İleti Kimliği** değeri görünen **Ayrıntılar** uçuş bölmesinde görünür.</span><span class="sxs-lookup"><span data-stu-id="22223-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="22223-109">Yöneticiler iletileri ve karşılık gelen İleti Kimliği değerlerini bulmak için [ileti izleme](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) sini kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="22223-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="22223-110">**Gönderen e-posta adresi**: Tek bir gönderenin e-posta adresi.</span><span class="sxs-lookup"><span data-stu-id="22223-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="22223-111">**Alıcı nın e-posta adresi**: Tek bir alıcının e-posta adresi.</span><span class="sxs-lookup"><span data-stu-id="22223-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="22223-112">**Konu**: İletinin tüm konusunu kullanın.</span><span class="sxs-lookup"><span data-stu-id="22223-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="22223-113">Arama büyük/küçük harf duyarlı değildir.</span><span class="sxs-lookup"><span data-stu-id="22223-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="22223-114">Arama ölçütlerini girdikten ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) sonra, sonuçları filtrelemek için**Yenile** düğmesini tıklatın.  </span><span class="sxs-lookup"><span data-stu-id="22223-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="22223-115">İletileri ve dosyaları karantinada görüntülemek ve yönetmek için kullandığınız cmdletler şunlardır:</span><span class="sxs-lookup"><span data-stu-id="22223-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="22223-116">Sil-KarantinaMesajı</span><span class="sxs-lookup"><span data-stu-id="22223-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="22223-117">Dışa Aktarma-KarantinaMesajı</span><span class="sxs-lookup"><span data-stu-id="22223-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="22223-118">Get-KarantinaMesajı</span><span class="sxs-lookup"><span data-stu-id="22223-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="22223-119">[Önizleme-Karantina Mesajı](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Bu cmdlet'in SharePoint Online, OneDrive for Business veya Teams için ATP'den gelen kötü amaçlı yazılım dosyaları için değil, yalnızca mesajlar için olduğunu unutmayın.</span><span class="sxs-lookup"><span data-stu-id="22223-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="22223-120">Yayın-KarantinaMesajı</span><span class="sxs-lookup"><span data-stu-id="22223-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)