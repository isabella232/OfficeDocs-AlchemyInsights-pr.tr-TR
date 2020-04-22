---
title: Klasik SharePoint denetim günlüğü raporları
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741985"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="7cbe1-102">SharePoint ve OneDrive denetim günlükleri</span><span class="sxs-lookup"><span data-stu-id="7cbe1-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="7cbe1-103">SharePoint klasik Denetim günlükleri</span><span class="sxs-lookup"><span data-stu-id="7cbe1-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="7cbe1-104">SPO eski denetimi Birleşik Denetim Günlüğü'ne (UAL) geçirildi.</span><span class="sxs-lookup"><span data-stu-id="7cbe1-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="7cbe1-105">Tüm SPO eski denetim raporları artık UAL üzerinden desteklenecek ve eski denetim sinyalleri UAL'a geçirilmiştir.</span><span class="sxs-lookup"><span data-stu-id="7cbe1-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="7cbe1-106">Önemli değişiklikler:</span><span class="sxs-lookup"><span data-stu-id="7cbe1-106">Key changes:</span></span>

* <span data-ttu-id="7cbe1-107">Kırpma bir yetenek olarak kullanılabilir DeğİlDir.</span><span class="sxs-lookup"><span data-stu-id="7cbe1-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="7cbe1-108">Denetlemek için belirli olayları seçmek mevcut DeğİlDIR.</span><span class="sxs-lookup"><span data-stu-id="7cbe1-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="7cbe1-109">Varsayılan olarak kullanılabilir denetlenen olayların tam listesi için [bu belgeye](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) bakın.</span><span class="sxs-lookup"><span data-stu-id="7cbe1-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="7cbe1-110">**Özelleştirilmiş raporlar** altında **Konum** seçeneği kullanılabilir DeğİlDİr.</span><span class="sxs-lookup"><span data-stu-id="7cbe1-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="7cbe1-111">**Belgeleri açma veya indirme** olayı seçeneği kullanılamıyor.</span><span class="sxs-lookup"><span data-stu-id="7cbe1-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="7cbe1-112">Site koleksiyonu için Denetim ayarlarını yapılandırma</span><span class="sxs-lookup"><span data-stu-id="7cbe1-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="7cbe1-113">Uyumluluktan SharePoint ve OneDrive Modern Birleşik Denetim günlükleri</span><span class="sxs-lookup"><span data-stu-id="7cbe1-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="7cbe1-114">Birleşik Denetim Günlüğe Kaydetme/Kapatma</span><span class="sxs-lookup"><span data-stu-id="7cbe1-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="7cbe1-115">SharePoint veya OneDrive içinde ek yapılandırma gerekmez.</span><span class="sxs-lookup"><span data-stu-id="7cbe1-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="7cbe1-116">Dosya(lar), klasör(ler), kullanıcı(lar), izinlerin etkinliğini denetlemek için denetim günlüğü aramasını kullanın:</span><span class="sxs-lookup"><span data-stu-id="7cbe1-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="7cbe1-117">Dosya ve sayfa etkinlikleri</span><span class="sxs-lookup"><span data-stu-id="7cbe1-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="7cbe1-118">Klasör etkinlikleri</span><span class="sxs-lookup"><span data-stu-id="7cbe1-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="7cbe1-119">İstek etkinliklerini paylaşma ve erişim</span><span class="sxs-lookup"><span data-stu-id="7cbe1-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="7cbe1-120">Senkronizasyon etkinlikleri</span><span class="sxs-lookup"><span data-stu-id="7cbe1-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="7cbe1-121">Site yönetimi faaliyetleri</span><span class="sxs-lookup"><span data-stu-id="7cbe1-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="7cbe1-122">Bu olayların nasıl alınabildiğini hakkında daha fazla bilgi için [denetim günlüğüne ara'ya](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)bakın.</span><span class="sxs-lookup"><span data-stu-id="7cbe1-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
