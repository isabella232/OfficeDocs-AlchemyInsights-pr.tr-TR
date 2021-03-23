---
title: Bildirim AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037233"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="da936-102">Bildirim AAD Connect</span><span class="sxs-lookup"><span data-stu-id="da936-102">Notification AAD Connect</span></span>

- <span data-ttu-id="da936-103">İşlem gerçekleştirmek için yetkili olduğundan emin olmak.</span><span class="sxs-lookup"><span data-stu-id="da936-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="da936-104">Genel Yöneticilerin varsayılan olarak erişimi vardır.</span><span class="sxs-lookup"><span data-stu-id="da936-104">Global Admins have access by default.</span></span> <span data-ttu-id="da936-105">Buna ek olarak, Katılımcıya [kayıt iznini temsilci olarak](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) temsil etmek için Rol Tabanlı Erişim Denetimi'i de kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="da936-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="da936-106">Gerekli uç noktaların etkinleştirildiğinden ve güvenlik duvarı nedeniyle engellenmiş olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="da936-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="da936-107">Ayrıntılar için gereksinimlere [bakın.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="da936-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="da936-108">Giden iletişim ağ katmanı tarafından SSL incelemesine tabi olduğu için kayıt başarısız olabilir.</span><span class="sxs-lookup"><span data-stu-id="da936-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="da936-109">Azure AD Connect Health için bildirim ayarlarını doğruladıktan emin olun ve ayarınızı gözden geçirin.</span><span class="sxs-lookup"><span data-stu-id="da936-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="da936-110">Azure AD Connect Durum bildirimleri için bildirim ayarlarını yapılandırmayı anlamak için bu kılavuza [bakın.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)</span><span class="sxs-lookup"><span data-stu-id="da936-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="da936-111">AAD Connect Durum eşitleme raporu ve nasıl indirildi hakkında daha fazla bilgi edinmek için, Nesne düzeyi [eşitleme raporuna bakın.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="da936-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="da936-112">AAD Connect Durum Uyarıları sorunlarını gidermek [için, AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Health veri tazeliği uyarılarının sorun giderme kılavuzuna bakın ve sık sorulan sorular için Genel [AAD Connect Durumu yükleme sorularına bakın.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="da936-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
