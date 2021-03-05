---
title: AAD Connect Health ile ilgili sorun
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483123"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="85854-102">AAD Connect Health ile ilgili sorun</span><span class="sxs-lookup"><span data-stu-id="85854-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="85854-103">İşlem gerçekleştirmek için yetkiniz olduğundan emin olmak.</span><span class="sxs-lookup"><span data-stu-id="85854-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="85854-104">Genel Yöneticilerin varsayılan olarak erişimi vardır.</span><span class="sxs-lookup"><span data-stu-id="85854-104">Global Admins have access by default.</span></span> <span data-ttu-id="85854-105">Buna ek olarak, Rol Tabanlı [Erişim Denetimi'i kullanarak Katılımcıya](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) kayıt iznini temsilci olarak devredebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="85854-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="85854-106">Gerekli uç noktaların etkinleştirildiğinden ve güvenlik duvarı nedeniyle engellenmiş olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="85854-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="85854-107">Ayrıntılar için gereksinimlere [bakın.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="85854-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="85854-108">Giden iletişim ağ katmanı tarafından SSL incelemesine tabi olduğu için kayıt başarısız olabilir.</span><span class="sxs-lookup"><span data-stu-id="85854-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="85854-109">Azure AD Connect Health için bildirim ayarlarını doğruladıktan emin olun.</span><span class="sxs-lookup"><span data-stu-id="85854-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="85854-110">Lütfen ayarınızı gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="85854-110">Please review your setting.</span></span> <span data-ttu-id="85854-111">Bu [kılavuz,](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) Azure AD Connect durum bildirimleri için bildirim ayarlarını yapılandırmayı anlamanıza yardımcı olabilir.</span><span class="sxs-lookup"><span data-stu-id="85854-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="85854-112">AAD Connect Durum eşitleme raporu ve nasıl indirildi hakkında daha fazla bilgi edinmek için, Nesne düzeyi [eşitleme raporuna bakın.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="85854-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="85854-113">AAD Connect Health uyarılarının sorunlarını gidermek [için, AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Health veri tazeliği uyarıları için sorun giderme kılavuzunu izleyin ve sık sorulan sorular için Genel AAD Connect Health yükleme [sorularına bakın.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="85854-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
