---
title: S/MIME Outlook web üzerinde
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666860"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="8e5bc-102">Outlook'ta e-posta iletileri şifreleme</span><span class="sxs-lookup"><span data-stu-id="8e5bc-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="8e5bc-103">Office 365 ileti şifreleme Microsoft Azure hakları Azure bilgi koruma parçası olan Yönetim üzerinde (Azure RMS) yerleşik olarak bulunur.</span><span class="sxs-lookup"><span data-stu-id="8e5bc-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="8e5bc-104">Aboneliğinizi Azure hak yönetimi veya Azure bilgi koruma, Rights Management hizmeti **el ile etkinleştirmeniz veya etkinleştirmek için herhangi bir eylem gerçekleştirmenizi gerekmez** içeriyorsa.</span><span class="sxs-lookup"><span data-stu-id="8e5bc-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="8e5bc-105">Müşteri görüşleri doğrultusunda, biz artık otomatik olarak varsayılan olarak belirli türde, Kiracı, hassas bilgilerin bulunduğu Giden e-posta şifrelemek Exchange posta akışı kurallarını etkinleştirmez.</span><span class="sxs-lookup"><span data-stu-id="8e5bc-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="8e5bc-106">Bunun yerine, biz nasıl bunu yapabilirsiniz hakkında ayrıntılı yönergeler sağlanmaktadır yourselves.</span><span class="sxs-lookup"><span data-stu-id="8e5bc-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="8e5bc-107">Önemli bilgileri şifrelemek için taşıma kuralının nasıl oluşturulacağı hakkında daha fazla ayrıntı için [Bu makaleye](https://aka.ms/OmeEtr)bakın.</span><span class="sxs-lookup"><span data-stu-id="8e5bc-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="8e5bc-108">Outlook Web (Eskiden **OWA**) kullanıyorsanız: bir e-posta iletisi oluştururken, OWA'ya **Koru** tıklatmanız yeterlidir.</span><span class="sxs-lookup"><span data-stu-id="8e5bc-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="8e5bc-109">Bu izni "iletme yapın" uygulanır.</span><span class="sxs-lookup"><span data-stu-id="8e5bc-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="8e5bc-110">**İzni değiştir'i** tıklatın ve yalnızca iletiyi şifrelemek için **şifreleme** seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="8e5bc-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="8e5bc-111">**Outlook istemcisi**kullanıyorsanız: Mac için Outlook 2013 veya 2016 veya Outlook 2016 şifreli ileti göndermek için **seçenekleri**seçin > **izinleri**, sonra da gereksinim duyduğunuz koruma seçeneğini seçin.</span><span class="sxs-lookup"><span data-stu-id="8e5bc-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="8e5bc-112">Belirli alıcılar veya dış ortak kuruluşlar için gönderilen **tüm e-posta otomatik olarak şifrelemek** için Exchange Yönetim Merkezi'nde posta akışını taşıma kuralı oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="8e5bc-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="8e5bc-113">[Bu destek makalesine](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)ayrıntılı yönergeler sağlanmıştır.</span><span class="sxs-lookup"><span data-stu-id="8e5bc-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

