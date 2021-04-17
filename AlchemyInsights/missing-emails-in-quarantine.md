---
title: Karantinada e-postalar eksik
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831754"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="78cf1-102">Karantinada e-postalar eksik"</span><span class="sxs-lookup"><span data-stu-id="78cf1-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="78cf1-103">Yöneticiler bu [iletileri görüntüde veya sürümde ilebilir veya silebilir.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="78cf1-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="78cf1-104">Güvenlik ve Uyumluluk & açmak için, [https://protection.office.com](https://protection.office.com/) gidin.</span><span class="sxs-lookup"><span data-stu-id="78cf1-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="78cf1-105">Karantina sayfasını doğrudan açmak için, [https://protection.office.com/quarantine](https://protection.office.com/quarantine) gidin.</span><span class="sxs-lookup"><span data-stu-id="78cf1-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="78cf1-106">Aşağıdaki değerlere göre arama yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="78cf1-106">You can search by the following values:</span></span>  

- <span data-ttu-id="78cf1-107">**İleti Kimliği:** İletinin genel benzersiz tanımlayıcısıdır.</span><span class="sxs-lookup"><span data-stu-id="78cf1-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="78cf1-108">Listeden bir ileti seçersiniz,  **görüntülenen**  Ayrıntılar açılır bölmesinde  **İleti**  Kimliği değeri gösterilir.</span><span class="sxs-lookup"><span data-stu-id="78cf1-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="78cf1-109">Yöneticiler, iletileri ve [karşılık gelen](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) İleti Kimliği değerlerini bulmak için ileti izleme kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="78cf1-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="78cf1-110">**Gönderen e-posta** adresi: Tek bir gönderenin e-posta adresi.</span><span class="sxs-lookup"><span data-stu-id="78cf1-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="78cf1-111">**Alıcı e-posta** adresi: Tek bir alıcının e-posta adresi.</span><span class="sxs-lookup"><span data-stu-id="78cf1-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="78cf1-112">**Konu:** İletinin konusunun tamamını kullanın.</span><span class="sxs-lookup"><span data-stu-id="78cf1-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="78cf1-113">Arama büyük/harfe duyarlı değildir.</span><span class="sxs-lookup"><span data-stu-id="78cf1-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="78cf1-114">Arama ölçütlerini girdikten sonra, sonuçları filtrelemek ![ için Yenile ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  düğmesini Yenile'yi tıklatın.  </span><span class="sxs-lookup"><span data-stu-id="78cf1-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="78cf1-115">Karantinada iletileri ve dosyaları görüntülemek ve yönetmek için kullanabileceğiniz cmdlet'ler:</span><span class="sxs-lookup"><span data-stu-id="78cf1-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="78cf1-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="78cf1-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="78cf1-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="78cf1-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="78cf1-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="78cf1-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="78cf1-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Bu cmdlet'in yalnızca iletilere yönelik olduğunu unutmayın; SharePoint Online, OneDrive İş veya Teams için ATP'den gelen kötü amaçlı yazılım dosyaları için değildir.</span><span class="sxs-lookup"><span data-stu-id="78cf1-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="78cf1-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="78cf1-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)