---
title: Sağlama hizmetini yapılandırma
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484047"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="6593d-102">Sağlama hizmetini yapılandırma</span><span class="sxs-lookup"><span data-stu-id="6593d-102">Configuring the Provision service</span></span>

<span data-ttu-id="6593d-103">Otomatik kullanıcı sağlamanın çalışması için, Azure AD'nin İşGünü Web Hizmetleri API'sine bağlanmasını sağlayan geçerli kimlik bilgileri gerekir.</span><span class="sxs-lookup"><span data-stu-id="6593d-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="6593d-104">Ayrıca, İşGünü'nden AD Kullanıcı Hazırlama uygulamasına yönelik Test Bağlantısı düğmesi, AD Etki Alanı ile ilişkilendirilmiş Azure AD Connect Sağlama Aracısına bağlananın mümkün olup olduğunu da doğrular.</span><span class="sxs-lookup"><span data-stu-id="6593d-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="6593d-105">Azure portalı kimlik bilgilerini kaydettikten sonra hata döndür kaydediliyorsa, aşağıdaki önerilen adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="6593d-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="6593d-106">İşGünü'de tümleştirme sistemi kullanıcılarını yapılandırma öğretici bölümünde belirtildiği gibi İşGünü Tümleştirme Sistemi Kullanıcı hesabını [yapılandırmış olduğunu onaylayın.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="6593d-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="6593d-107">Hizmetler Yönetim Konsolu'nu kullanarak şirket içi Windows sunucunuzda Azure AD Connect Sağlama Aracı Hizmeti'nin çalışır ve çalışır olduğunu onaylayın.</span><span class="sxs-lookup"><span data-stu-id="6593d-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="6593d-108">Ayrıca, Şirket içi aracıları görüntüle düğmesine tıklayarak Azure portalında aracının durumunu da kontrol edebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6593d-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="6593d-109">Kiracı-adı biçimini kullanarak "İşGünü Kullanıcı Adı" alanı değerini username@workday emin olun.</span><span class="sxs-lookup"><span data-stu-id="6593d-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="6593d-110">İşgünü kiracı adı yoksa, İşGünü kimlik doğrulaması başarısız olur.</span><span class="sxs-lookup"><span data-stu-id="6593d-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="6593d-111">İşGünü uygulama kiracısı ile tümleştirmeyi yapılandırıyorsanız, İşGünü kiracınıza yönelik zamanlanmış kapalı kalma saatlerini not edersiniz.</span><span class="sxs-lookup"><span data-stu-id="6593d-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="6593d-112">İşgünü, uygulama kiracıları için hafta sonları (çoğunlukla Cuma akşamdan Cumartesi sabahına kadar) zamanlanmış ve bu kesinti süresi boyunca bağlantı hataları, uygulama kiracıları yeniden çevrimiçi olur dönmez otomatik olarak çözülen bilinen bir sorundur.</span><span class="sxs-lookup"><span data-stu-id="6593d-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="6593d-113">Ender durumlarda, Tümleştirme Sistemi Kullanıcısı parolasının kiracı yenilemesi nedeniyle değişmesi veya hesabın kilitli veya süresinin dolması durumu nedeniyle bu hatayı da alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6593d-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="6593d-114">Lütfen İşGünü yöneticinizle Tümleştirme Sistemi kullanıcılarının durumunu kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="6593d-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="6593d-115">Otomatik sağlama için iş günü yapılandırma hakkında daha fazla ayrıntı için öğreticiye bakın: Otomatik kullanıcı [sağlama için İşGünü'ne yapılandırma.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="6593d-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
