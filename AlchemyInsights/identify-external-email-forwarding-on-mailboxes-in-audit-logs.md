---
title: Dış e-posta İletim Denetim günlüklerini de posta kutuları belirle
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417231"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="1d36e-102">Dış e-posta iletme posta kutuları üzerinde yapılandırıldığında belirle</span><span class="sxs-lookup"><span data-stu-id="1d36e-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="1d36e-103">Bir kullanıcı bir posta kutusuna dış e-posta iletme yapılandırır, etkinlik **Kümesi-posta kutusu** cmdlet'i bir parçası olarak denetlenir.</span><span class="sxs-lookup"><span data-stu-id="1d36e-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="1d36e-104">Güvenlik & Uyumluluk Merkezi Denetim günlüğü aramayı kullanarak etkinliğini görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="1d36e-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="1d36e-105">Oturum [Office 365 güvenlik & Uyumluluk Merkezi](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="1d36e-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="1d36e-106">**Arama ve araştırma'yı** tıklatın ve **Denetim günlüğü Ara**' yı seçin.</span><span class="sxs-lookup"><span data-stu-id="1d36e-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="1d36e-107">**Başlangıç tarihi** ve **Bitiş tarihi** alanlarında tarih aralığını seçin.</span><span class="sxs-lookup"><span data-stu-id="1d36e-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="1d36e-108">Bir kullanıcı adı belirtmeniz gerekmez.</span><span class="sxs-lookup"><span data-stu-id="1d36e-108">You don't need to specify a username.</span></span> <span data-ttu-id="1d36e-109">**Tüm etkinlikler için sonuçları göstermek**için **etkinlikler** alanı olarak doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="1d36e-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="1d36e-110">**Ara**' yı tıklatın.</span><span class="sxs-lookup"><span data-stu-id="1d36e-110">Click **Search**.</span></span>

<span data-ttu-id="1d36e-111">Sonuçları **Filtre sonuçları** ' nı tıklatın ve **Set-posta kutusu** etkinlik filtre kutusunda yazın.</span><span class="sxs-lookup"><span data-stu-id="1d36e-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="1d36e-112">Sonuçları bir denetim kaydı seçin.</span><span class="sxs-lookup"><span data-stu-id="1d36e-112">Select an audit record in the results.</span></span> <span data-ttu-id="1d36e-113">**Daha fazla bilgi** **Ayrıntılar** çıkma içinde tıklatın.</span><span class="sxs-lookup"><span data-stu-id="1d36e-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="1d36e-114">Etkinlik iletme ilişkili olup olmadığını belirlemek için her bir denetim kaydı ayrıntılara bakmak zorunda.</span><span class="sxs-lookup"><span data-stu-id="1d36e-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="1d36e-115">**NesneKimliği**: diğer ad değeri değiştirilmiş olan posta kutusu.</span><span class="sxs-lookup"><span data-stu-id="1d36e-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="1d36e-116">**Parametreler**: _ForwardingSmtpAddress_ hedef e-posta adresini gösterir.</span><span class="sxs-lookup"><span data-stu-id="1d36e-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="1d36e-117">**Kullanıcı kimliği**: **NesneKimliği** alanında posta kutusu e-posta iletme yapılandırılmış kullanıcı.</span><span class="sxs-lookup"><span data-stu-id="1d36e-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="1d36e-118">Daha fazla bilgi için bkz: [belirleme kimin e-posta iletmek için bir posta kutusu ayarlayın](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="1d36e-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>