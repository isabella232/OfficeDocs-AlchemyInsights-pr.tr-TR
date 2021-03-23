---
title: Yammer'dan içeri ve dışarı aktarma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037255"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="7b769-102">Yammer'dan içeri ve dışarı aktarma</span><span class="sxs-lookup"><span data-stu-id="7b769-102">Import and export from Yammer</span></span>

<span data-ttu-id="7b769-103">**İçeri aktar**</span><span class="sxs-lookup"><span data-stu-id="7b769-103">**Import**</span></span>

<span data-ttu-id="7b769-104">Kullanıcı içeri aktarma seçenekleri, Yammer ağınızı [Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)için Yerel Modda olup olmadığınıza bağlı olarak değişir.</span><span class="sxs-lookup"><span data-stu-id="7b769-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="7b769-105">**Yerel Olmayan Mod:** Kullanıcılar, Grup ayarları içinde Adres Defteri'den [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) [Ekle](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) 'yi kullanarak gruplara (100 kullanıcıyla sınırla) veya Ağ Yöneticisi içindeki Toplu Güncelleştirme kullanılarak ağa aktarabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="7b769-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="7b769-106">**Yerel Mod:** Grup üyeliği ve ağ üyeliği işlemleri [Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users)yönetim portalında, [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)portalında veya başka bir Azure AD seçeneği kullanılarak yapılmalıdır.</span><span class="sxs-lookup"><span data-stu-id="7b769-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="7b769-107">Yerel Mod'daki ağların artık Toplu Güncelleştirme ve diğer eski özelliklere erişimi yoktur.</span><span class="sxs-lookup"><span data-stu-id="7b769-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7b769-108">Yammer, Veri Dışarı Aktarma özelliği başka bir ağda kullanılmış olsa bile Ağ Yöneticisi'nin içinde içerik içeri aktarmayı hiçbir zaman desteklemez.</span><span class="sxs-lookup"><span data-stu-id="7b769-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="7b769-109">İçerik iş ortağı çözümleri veya Yammer REST API'leri tarafından yeniden posta olabilir.</span><span class="sxs-lookup"><span data-stu-id="7b769-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="7b769-110">**Dışarı Aktar**</span><span class="sxs-lookup"><span data-stu-id="7b769-110">**Export**</span></span>

<span data-ttu-id="7b769-111">[Ağ Verilerini Ağ Yöneticisi'nin içinde](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) dışarı aktarma, iletiler ve dosyalar dahil olmak üzere Yammer ağlarından içerik dışarı aktarmaya izin verir.</span><span class="sxs-lookup"><span data-stu-id="7b769-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="7b769-112">Ekler aşırı büyük olabilir ve dışarı aktarma işleminin tamamlanması önemli ölçüde zaman alır.</span><span class="sxs-lookup"><span data-stu-id="7b769-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="7b769-113">Etkin ağların, Veri Dışarı Aktarma [API'si](https://developer.yammer.com/docs/data-export-api) kullanılarak gün veya haftaya göre parçalar halinde dışarı aktarmasını öneririz.</span><span class="sxs-lookup"><span data-stu-id="7b769-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="7b769-114">Microsoft Desteği bu amaç için özel betikler sağlamaz.</span><span class="sxs-lookup"><span data-stu-id="7b769-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="7b769-115">Tek bir [kullanıcının içeriğini dışarı aktaran](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) ayrı bir GDPR dışarı aktarma vardır.</span><span class="sxs-lookup"><span data-stu-id="7b769-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>