---
title: Karantinadaki e-postalar eksik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673734"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="7d3ca-102">Karantinadaki e-postalar eksik "</span><span class="sxs-lookup"><span data-stu-id="7d3ca-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="7d3ca-103">Yöneticiler [Bu iletileri görüntüleyebilir, serbest bırakabilir veya silebilir.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="7d3ca-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="7d3ca-104">Güvenlik & Uyumluluk Merkezi 'ni açmak için gidin [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="7d3ca-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="7d3ca-105">Karantina sayfasını doğrudan açmak için öğesine gidin [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="7d3ca-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="7d3ca-106">Aşağıdaki değerlerle arama yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="7d3ca-106">You can search by the following values:</span></span>  

- <span data-ttu-id="7d3ca-107">**ILETI kimliği**: iletinin genel benzersiz tanımlayıcısı.</span><span class="sxs-lookup"><span data-stu-id="7d3ca-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="7d3ca-108">Listeden bir ileti seçerseniz, görüntülenen **Ayrıntılar** açılır BÖLMESINDE **ileti kimliği** değeri görünür.</span><span class="sxs-lookup"><span data-stu-id="7d3ca-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="7d3ca-109">Yöneticiler ileti [izlemeyi](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) kullanarak iletileri ve ılgılı ileti kimliği değerlerini bulabilir.</span><span class="sxs-lookup"><span data-stu-id="7d3ca-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="7d3ca-110">**Gönderenin e-posta adresi**: tek bir gönderenin e-posta adresi.</span><span class="sxs-lookup"><span data-stu-id="7d3ca-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="7d3ca-111">**Alıcının e-posta adresi**: tek bir alıcının e-posta adresi.</span><span class="sxs-lookup"><span data-stu-id="7d3ca-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="7d3ca-112">**Konu**: iletinin tüm konusunu kullanın.</span><span class="sxs-lookup"><span data-stu-id="7d3ca-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="7d3ca-113">Arama büyük/küçük harf duyarlı değildir.</span><span class="sxs-lookup"><span data-stu-id="7d3ca-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="7d3ca-114">Arama ölçütlerini girdikten sonra, ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) sonuçları filtrelemek için Yenile düğmesini**Yenile** 'yi tıklatın.  </span><span class="sxs-lookup"><span data-stu-id="7d3ca-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="7d3ca-115">İletileri ve karantinadaki dosyaları görüntülemek ve yönetmesi için kullandığınız cmdlet 'ler:</span><span class="sxs-lookup"><span data-stu-id="7d3ca-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="7d3ca-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="7d3ca-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="7d3ca-117">Dışarı aktarma-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="7d3ca-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="7d3ca-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="7d3ca-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="7d3ca-119">[Önizleme-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Bu cmdlet 'in yalnızca iletiler için olduğunu, SharePoint Online, OneDrive Iş veya ekiplerin ATP 'den kötü amaçlı yazılım dosyaları olmadığını unutmayın.</span><span class="sxs-lookup"><span data-stu-id="7d3ca-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="7d3ca-120">Sürüm karantinaya alır</span><span class="sxs-lookup"><span data-stu-id="7d3ca-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)