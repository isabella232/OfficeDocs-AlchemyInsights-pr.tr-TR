---
title: Denetim günlüklerindeki posta kutularındaki dış e-posta iletmeyi tanımlama
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696317"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="044d9-102">Posta kutularında dış e-posta iletme 'nin ne zaman yapılandırıldığını belirleme</span><span class="sxs-lookup"><span data-stu-id="044d9-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="044d9-103">Bir Microsoft 365 kullanıcısı posta kutusunda dış e-posta iletmeyi yapılandırırsa, etkinlik, **Set-Mailbox** cmdlet 'inin bir parçası olarak denetlenir.</span><span class="sxs-lookup"><span data-stu-id="044d9-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="044d9-104">Güvenlik & Uyumluluk Merkezi 'nde denetim günlüğü aramasını kullanarak etkinliği görebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="044d9-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="044d9-105">[Microsoft 365 güvenlik & Uyumluluk Merkezi](https://protection.office.com/)'nde oturum açın.</span><span class="sxs-lookup"><span data-stu-id="044d9-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="044d9-106">**Search**  >  **Denetim günlüğü aramasını** ara sayfasına gidin.</span><span class="sxs-lookup"><span data-stu-id="044d9-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="044d9-107">**Başlangıç tarihi** ve **bitiş tarihi** alanlarında tarih aralığını seçin.</span><span class="sxs-lookup"><span data-stu-id="044d9-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="044d9-108">Kullanıcı adı belirtmeniz gerekmez.</span><span class="sxs-lookup"><span data-stu-id="044d9-108">You don't need to specify a username.</span></span> <span data-ttu-id="044d9-109">**Etkinlikler** alanının **tüm etkinlikler için sonuçları gösterecek**şekilde ayarlandığını doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="044d9-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="044d9-110">**Ara**'ya tıklayın.</span><span class="sxs-lookup"><span data-stu-id="044d9-110">Click **Search**.</span></span>

<span data-ttu-id="044d9-111">Sonuçlarda, **Sonuçları filtrele** 'ye tıklayın ve etkinlik filtresi kutusuna **Set-Mailbox** yazın.</span><span class="sxs-lookup"><span data-stu-id="044d9-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="044d9-112">Sonuçlarda bir denetim kaydı seçin.</span><span class="sxs-lookup"><span data-stu-id="044d9-112">Select an audit record in the results.</span></span> <span data-ttu-id="044d9-113">**Ayrıntılar** açılır listesinde, **ek bilgi**'yi tıklatın.</span><span class="sxs-lookup"><span data-stu-id="044d9-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="044d9-114">Etkinliğin e-posta iletme ile ilgili olup olmadığını belirlemek için her bir denetim kaydının ayrıntılarına bakmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="044d9-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="044d9-115">**ObjectID**: değiştirilmiş olan posta kutusunun diğer ad değeri.</span><span class="sxs-lookup"><span data-stu-id="044d9-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="044d9-116">**Parametreler**: _ForwardingSMTPAddress_ hedef e-posta adresini gösterir.</span><span class="sxs-lookup"><span data-stu-id="044d9-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="044d9-117">**Kullanıcı kimliği**: **ObjectID** alanındaki posta kutusunda e-postayı ileten Kullanıcı.</span><span class="sxs-lookup"><span data-stu-id="044d9-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="044d9-118">Daha fazla bilgi için, [posta kutusu için e-posta iletmeyi kimlerin görebileceğini belirleme](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)konusuna bakın.</span><span class="sxs-lookup"><span data-stu-id="044d9-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
