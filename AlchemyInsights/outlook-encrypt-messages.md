---
title: Web üzerinde Outlook 'ta S/MIME
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772318"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="b316b-102">Outlook 'ta e-posta iletilerini şifreleme</span><span class="sxs-lookup"><span data-stu-id="b316b-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="b316b-103">Microsoft 365 Ileti şifreleme, Azure Information Protection 'ın bir parçası olan Microsoft Azure Rights Management (Azure RMS) üzerine kurulmuştur.</span><span class="sxs-lookup"><span data-stu-id="b316b-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="b316b-104">Aboneliğiniz Azure Rights Management veya Azure Information Protection içeriyorsa, hak yönetimi hizmetini **etkinleştirmek veya etkinleştirmek için herhangi bir işlem yapmanız gerekmez** .</span><span class="sxs-lookup"><span data-stu-id="b316b-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="b316b-105">Müşteri geri bildirimlerine bağlı olarak, varsayılan olarak kiracınızda belirli tür duyarlı bilgileri içeren giden e-postayı otomatik olarak şifreleyemiyoruz.</span><span class="sxs-lookup"><span data-stu-id="b316b-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="b316b-106">Bunun yerine yourselves bunu nasıl yapabileceğiniz hakkında ayrıntılı yönergeler sunuyoruz.</span><span class="sxs-lookup"><span data-stu-id="b316b-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="b316b-107">Hassas bilgilerin şifrelenmesinde bir taşıma kuralı oluşturma hakkında ek bilgi için [Bu makaleye](https://aka.ms/OmeEtr)bakın.</span><span class="sxs-lookup"><span data-stu-id="b316b-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="b316b-108">Web üzerinde Outlook (eski adı **OWA**) kullanılıyorsa: e-posta iletisi oluştururken, yalnızca OWA 'da **korumayı** tıklatın.</span><span class="sxs-lookup"><span data-stu-id="b316b-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="b316b-109">"İletme" izni uygulanır.</span><span class="sxs-lookup"><span data-stu-id="b316b-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="b316b-110">**Izni Değiştir** 'i tıklatın ve yalnızca iletiyi şifrelemek için **şifrele** 'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="b316b-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="b316b-111">**Outlook istemcisi**kullanılıyorsa: Outlook 2013 veya 2016 veya Mac için Outlook 2016 ' den şifrelenmiş bir ileti göndermek için **Seçenekler**  >  **izinler**'i seçin ve sonra da ihtiyacınız olan koruma seçeneğini belirleyin.</span><span class="sxs-lookup"><span data-stu-id="b316b-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="b316b-112">Belirli alıcılara veya dış iş ortağı kuruluşlara gönderilen **tüm e-postaları otomatik olarak şifrelemek** Için, Exchange Yönetim merkezinde bir posta akışı aktarım kuralı oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="b316b-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="b316b-113">Ayrıntılı yönergeler [Bu destek makalesinde](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)sağlanmaktadır.</span><span class="sxs-lookup"><span data-stu-id="b316b-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

