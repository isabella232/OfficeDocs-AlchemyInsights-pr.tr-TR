---
title: Klasik SharePoint denetim günlüğü raporları
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068043"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="558c1-102">SharePoint ve OneDrive denetim günlükleri</span><span class="sxs-lookup"><span data-stu-id="558c1-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="558c1-103">**Uyumluluktan SharePoint ve OneDrive Modern Birleşik Denetim günlükleri**</span><span class="sxs-lookup"><span data-stu-id="558c1-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="558c1-104">Birleşik Denetim Günlüğe Kaydetme/Kapatma</span><span class="sxs-lookup"><span data-stu-id="558c1-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="558c1-105">SharePoint veya OneDrive içinde ek yapılandırma gerekmez.</span><span class="sxs-lookup"><span data-stu-id="558c1-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="558c1-106">Dosya(lar), klasör(ler), kullanıcı(lar), izinlerin etkinliğini denetlemek için denetim günlüğü aramasını kullanın:</span><span class="sxs-lookup"><span data-stu-id="558c1-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="558c1-107">Dosya ve sayfa etkinlikleri</span><span class="sxs-lookup"><span data-stu-id="558c1-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="558c1-108">Klasör etkinlikleri</span><span class="sxs-lookup"><span data-stu-id="558c1-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="558c1-109">İstek etkinliklerini paylaşma ve erişim</span><span class="sxs-lookup"><span data-stu-id="558c1-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="558c1-110">Senkronizasyon etkinlikleri</span><span class="sxs-lookup"><span data-stu-id="558c1-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="558c1-111">Site yönetimi faaliyetleri</span><span class="sxs-lookup"><span data-stu-id="558c1-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="558c1-112">Bu olayların nasıl alınabildiğini hakkında daha fazla bilgi için [denetim günlüğüne ara'ya](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)bakın.</span><span class="sxs-lookup"><span data-stu-id="558c1-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="558c1-113">**SharePoint klasik Denetim günlükleri**</span><span class="sxs-lookup"><span data-stu-id="558c1-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="558c1-114">SPO eski denetimini Birleşik Denetim Günlüğü'ne (UAL) ilettik.</span><span class="sxs-lookup"><span data-stu-id="558c1-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="558c1-115">Bu temelde tüm SPO eski denetim raporları artık UAL üzerinden güçlendirilmiş olacak ve eski denetim sinyalleri UAL'a geçirilmiştir anlamına gelir.</span><span class="sxs-lookup"><span data-stu-id="558c1-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="558c1-116">Önemli değişiklikler:</span><span class="sxs-lookup"><span data-stu-id="558c1-116">Key changes:</span></span>

- <span data-ttu-id="558c1-117">Bir yetenek olarak kırpma mevcut DeğİlDIR.</span><span class="sxs-lookup"><span data-stu-id="558c1-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="558c1-118">Denetlemek için belirli olayları seçtiğiniz bölüm MEVCUT DeğİlDIR.</span><span class="sxs-lookup"><span data-stu-id="558c1-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="558c1-119">Varsayılan olarak kullanılabilir denetlenen olayların tam listesi için lütfen [bu belgeye](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) bakın.</span><span class="sxs-lookup"><span data-stu-id="558c1-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="558c1-120">**Özelleştirilmiş raporlar** altında "Konum" seçeneği kullanılabilir DeğİlDİr.</span><span class="sxs-lookup"><span data-stu-id="558c1-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="558c1-121">"Belgeleri açma veya indirme" etkinlikleri MEVCUT DeğİlDİr.</span><span class="sxs-lookup"><span data-stu-id="558c1-121">“Opening or downloading documents” events is NOT available.</span></span> 

