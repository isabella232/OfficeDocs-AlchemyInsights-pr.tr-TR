---
title: Klasik SharePoint denetim günlüğü raporları
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662228"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="5756a-102">SharePoint ve OneDrive denetim günlükleri</span><span class="sxs-lookup"><span data-stu-id="5756a-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="5756a-103">SharePoint klasik denetim günlükleri</span><span class="sxs-lookup"><span data-stu-id="5756a-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="5756a-104">SPO eski denetim Birleşik denetim günlüğüne (sürekli) geçirildi.</span><span class="sxs-lookup"><span data-stu-id="5756a-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="5756a-105">Tüm SPO eski denetim raporları artık sürekli kalacak ve eski denetim sinyalleri sürekli olarak geçirilir.</span><span class="sxs-lookup"><span data-stu-id="5756a-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="5756a-106">Anahtar değişiklikleri:</span><span class="sxs-lookup"><span data-stu-id="5756a-106">Key changes:</span></span>

* <span data-ttu-id="5756a-107">Kırpma özelliği yetenek olarak kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="5756a-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="5756a-108">Denetlenecek belirli olayları seçme kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="5756a-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="5756a-109">Varsayılan olarak sağlanan denetlenen olayların tam listesi için [Bu belgeye](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) başvurun.</span><span class="sxs-lookup"><span data-stu-id="5756a-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="5756a-110">**Özelleştirilmiş raporlar** 'ın altındaki **konum** seçeneği kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="5756a-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="5756a-111">**Belge olaylarını açma veya indirme** seçeneği kullanılamaz.</span><span class="sxs-lookup"><span data-stu-id="5756a-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="5756a-112">Site koleksiyonu için denetim ayarlarını yapılandırma</span><span class="sxs-lookup"><span data-stu-id="5756a-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="5756a-113">Uyumluluk için SharePoint ve OneDrive modern denetim günlükleri</span><span class="sxs-lookup"><span data-stu-id="5756a-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="5756a-114">Birleşik denetim günlüğünü açma/kapatma</span><span class="sxs-lookup"><span data-stu-id="5756a-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="5756a-115">SharePoint veya OneDrive 'da ek yapılandırma gerekmez.</span><span class="sxs-lookup"><span data-stu-id="5756a-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="5756a-116">Dosya (lar), klasör, Kullanıcı (lar), izinler:</span><span class="sxs-lookup"><span data-stu-id="5756a-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="5756a-117">Dosya ve sayfa etkinlikleri</span><span class="sxs-lookup"><span data-stu-id="5756a-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="5756a-118">Klasör etkinlikleri</span><span class="sxs-lookup"><span data-stu-id="5756a-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="5756a-119">Paylaşım ve erişim isteği etkinlikleri</span><span class="sxs-lookup"><span data-stu-id="5756a-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="5756a-120">Eşitleme etkinlikleri</span><span class="sxs-lookup"><span data-stu-id="5756a-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="5756a-121">Site yönetimi etkinlikleri</span><span class="sxs-lookup"><span data-stu-id="5756a-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="5756a-122">Bu olayları geri alma hakkında daha fazla bilgi için [denetim günlüğünde arama](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="5756a-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
