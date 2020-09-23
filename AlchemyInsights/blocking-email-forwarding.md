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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219875"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="d2ed4-102">E-posta iletmeyi engelleme veya engellemeyi kaldırma</span><span class="sxs-lookup"><span data-stu-id="d2ed4-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="d2ed4-103">Belirli bir posta kutusu için e- [posta iletmeyi etkinleştirmek](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)veya devre dışı bırakmak için</span><span class="sxs-lookup"><span data-stu-id="d2ed4-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="d2ed4-104">Kiracı düzeyinde, dış iletme denetimi giden istenmeyen posta önleme ilkesi kullanılarak yapılır.</span><span class="sxs-lookup"><span data-stu-id="d2ed4-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="d2ed4-105">Kapalı veya otomatik olarak ayarlanmışsa, "550 5.7.520 erişimi reddedildi, kuruluşunuz dış iletmeye izin vermiyor" hatası ile e-posta iletmeyi engelleyebilir.</span><span class="sxs-lookup"><span data-stu-id="d2ed4-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="d2ed4-106">Ardından, yönlendirme engellenmiş olarak ayarlanmışsa, bu hata, kullanıcılarınızın göreceği hatadır.</span><span class="sxs-lookup"><span data-stu-id="d2ed4-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="d2ed4-107">İletme engellendiyse, lütfen ilkenin dış otomatik Iletimi etkinleştirecek şekilde yapılandırıldığından emin olun.</span><span class="sxs-lookup"><span data-stu-id="d2ed4-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="d2ed4-108">Giden Istenmeyen posta Filtresi Ilkesini güvenlik ve Uyumluluk Merkezi 'nden denetleyebilir veya Command-HostedOutboundSpamFilterPolicy | fl Name, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="d2ed4-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="d2ed4-109">Otomatik Iletme engellemesi 'ni ayarlamak istiyorsanız, ilkenin durumunu şimdi size bildirir.</span><span class="sxs-lookup"><span data-stu-id="d2ed4-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="d2ed4-110">Not: Varsayılan giden Istenmeyen posta Filtresi ilkeleriniz için dış otomatik Iletme devre dışı tutulmasını ve yalnızca bu kullanıcılar için özel bir ilke oluşturarak yalnızca dış yönlendirmeyi gerektiren kullanıcıları etkinleştirmesini öneririz.</span><span class="sxs-lookup"><span data-stu-id="d2ed4-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="d2ed4-111">[Office 365 ' de dış e-posta Iletmeyi yapılandırmada](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)daha fazlasını okuyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d2ed4-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>