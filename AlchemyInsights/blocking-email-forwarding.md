---
title: 726 e-posta iletmeyi engelliyor
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473121"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="6ef25-102">E-posta iletmeyi engelleme veya engellemeyi kaldırma</span><span class="sxs-lookup"><span data-stu-id="6ef25-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="6ef25-103">Belirli bir posta kutusu için e- [posta iletmeyi etkinleştirmek](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)veya devre dışı bırakmak için</span><span class="sxs-lookup"><span data-stu-id="6ef25-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="6ef25-104">Kiracı düzeyinde, dış iletme denetimi giden istenmeyen posta ilkesi kullanılarak yapılır.</span><span class="sxs-lookup"><span data-stu-id="6ef25-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="6ef25-105">Giden istenmeyen posta Filtresi politikasını güvenlik ve Uyumluluk Merkezi 'nden [burada] https://protection.office.com/antispam) veya [Get-HostedOutboundSpamFilterPolicy komutunu](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)kullanarak denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6ef25-105">You can check the outbound spam filter policy from Security and Compliance Center [here] (https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="6ef25-106">Aşağıdaki hatayı alıyorsanız: **"550 5.7.520 erişim reddedildi, kuruluşunuz dış iletmeye izin vermiyor"**, lütfen Ilkenin dış Otomatik iletmeyi etkinleştirecek şekilde yapılandırıldığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="6ef25-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="6ef25-107">**Not:** Varsayılan giden istenmeyen posta Filtresi ilkeleriniz için dış otomatik Iletme devre dışı tutulmasını ve yalnızca bu kullanıcılar için özel bir ilke oluşturarak yalnızca dış yönlendirmeyi gerektiren kullanıcıları etkinleştirmesini öneririz.</span><span class="sxs-lookup"><span data-stu-id="6ef25-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="6ef25-108">[Office 365 ' de dış e-posta Iletmeyi yapılandırmada](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)daha fazlasını okuyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="6ef25-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>