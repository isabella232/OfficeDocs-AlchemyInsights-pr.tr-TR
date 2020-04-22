---
title: Denetim günlüklerinde posta kutularında harici e-posta yönlendirmeyi tanımlama
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716480"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="92b6d-102">Posta kutularında harici e-posta yönlendirmenin ne zaman yapılandırılma da olduğunu belirleme</span><span class="sxs-lookup"><span data-stu-id="92b6d-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="92b6d-103">Bir Microsoft 365 kullanıcısı bir posta kutusunda harici e-posta yönlendirmeyi yapılandırırsa, etkinlik **Set-Posta Kutusu** cmdlet'in bir parçası olarak denetlenir.</span><span class="sxs-lookup"><span data-stu-id="92b6d-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="92b6d-104">Etkinliği Güvenlik & Uyumluluk Merkezi'nde denetim günlüğü aramasını kullanarak görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="92b6d-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="92b6d-105">[Microsoft 365 Güvenlik & Uyumluluk Merkezi'nde](https://protection.office.com/)oturum açın.</span><span class="sxs-lookup"><span data-stu-id="92b6d-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="92b6d-106">**Arama** > **Denetimi günlüğü arama** sayfasına gidin.</span><span class="sxs-lookup"><span data-stu-id="92b6d-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="92b6d-107">**Başlangıç tarihi** ve Bitiş **tarihi** alanlarındaki tarih aralığını seçin.</span><span class="sxs-lookup"><span data-stu-id="92b6d-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="92b6d-108">Bir kullanıcı adı belirtmeniz gerekmez.</span><span class="sxs-lookup"><span data-stu-id="92b6d-108">You don't need to specify a username.</span></span> <span data-ttu-id="92b6d-109">**Etkinlikler** alanının tüm **etkinliklerin sonuçlarını gösterecek**şekilde ayarlı olduğunu doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="92b6d-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="92b6d-110">**Arama'yı**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="92b6d-110">Click **Search**.</span></span>

<span data-ttu-id="92b6d-111">Sonuçlarda, **Sonuçları Filtrele'yi** ve etkinlik filtresi kutusunda **Set-Posta Kutusu** yazın'ı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="92b6d-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="92b6d-112">Sonuçlarda bir denetim kaydı seçin.</span><span class="sxs-lookup"><span data-stu-id="92b6d-112">Select an audit record in the results.</span></span> <span data-ttu-id="92b6d-113">**Ayrıntılar** flyout, **daha fazla bilgi**tıklatın.</span><span class="sxs-lookup"><span data-stu-id="92b6d-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="92b6d-114">Etkinliğin e-posta yönlendirmeyle ilgili olup olmadığını belirlemek için her denetim kaydının ayrıntılarına bakmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="92b6d-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="92b6d-115">**ObjectId**: Değiştirilen posta kutusunun diğer adı değeri.</span><span class="sxs-lookup"><span data-stu-id="92b6d-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="92b6d-116">**Parametreler**: _ForwardingSmtpAddress_ hedef e-posta adresini gösterir.</span><span class="sxs-lookup"><span data-stu-id="92b6d-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="92b6d-117">**UserId**: **ObjectId** alanında posta kutusunda e-posta yönlendirmeyi yapılandıran kullanıcı.</span><span class="sxs-lookup"><span data-stu-id="92b6d-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="92b6d-118">Daha fazla bilgi için [bkz.](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)</span><span class="sxs-lookup"><span data-stu-id="92b6d-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
