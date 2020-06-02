---
title: Web'de Outlook'ta S/MIME
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511528"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="fa92c-102">Outlook'ta e-posta iletilerini şifreleme</span><span class="sxs-lookup"><span data-stu-id="fa92c-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="fa92c-103">Microsoft 365 İleti Şifrelemesi, Azure Bilgi Koruması'nın bir parçası olan Microsoft Azure Hakları Yönetimi 'nde (Azure RMS) yerleşiktir.</span><span class="sxs-lookup"><span data-stu-id="fa92c-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="fa92c-104">Aboneliğiniz Azure Hakları Yönetimi veya Azure Bilgi Koruması içeriyorsa, Hak Yönetimi Hizmetini **el ile etkinleştirmek veya etkinleştirmek için herhangi bir işlem yapmanız gerekmez.**</span><span class="sxs-lookup"><span data-stu-id="fa92c-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="fa92c-105">Müşteri geri bildirimlerine dayanarak, exchange posta akışı kurallarının varsayılan olarak kiracınızda belirli türde hassas bilgiler içeren giden e-postaları otomatik olarak şifrelemesini etkinleştirmeyeceğiz.</span><span class="sxs-lookup"><span data-stu-id="fa92c-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="fa92c-106">Bunun yerine, bunu kendiniz nasıl yapabileceğinize ilişkin ayrıntılı talimatlar salıyoruz.</span><span class="sxs-lookup"><span data-stu-id="fa92c-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="fa92c-107">Hassas bilgileri şifrelemek için aktarım kuralının nasıl oluşturulacaaçık ayrıntılar için [bu makaleye](https://aka.ms/OmeEtr)bakın.</span><span class="sxs-lookup"><span data-stu-id="fa92c-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="fa92c-108">Outlook'u Web'de kullanıyorsanız (eski adıyla **OWA):** Bir e-posta iletisi oluştururken, OWA'da **Koru'yu** tıklatın.</span><span class="sxs-lookup"><span data-stu-id="fa92c-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="fa92c-109">Bu " İlerletme" izni geçerli olacaktır.</span><span class="sxs-lookup"><span data-stu-id="fa92c-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="fa92c-110">**İzin Değiştir'i** tıklatın ve yalnızca iletiyi şifrelemek için **Şifrele'yi** seçin.</span><span class="sxs-lookup"><span data-stu-id="fa92c-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="fa92c-111">Outlook **istemcisini**kullanıyorsanız : Outlook 2013 veya 2016'dan veya Mac için Outlook 2016'dan şifreli ileti göndermek için **Seçenekler**  >  **İzinleri'ni**seçin ve ardından ihtiyacınız olan koruma seçeneğini seçin.</span><span class="sxs-lookup"><span data-stu-id="fa92c-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="fa92c-112">Belirli alıcılara veya dış iş ortağı kuruluşlarına gönderilen **tüm e-postaları otomatik olarak şifrelemek** için Exchange Yönetici Merkezi'nde bir posta akışı aktarım kuralı oluşturmanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="fa92c-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="fa92c-113">Ayrıntılı talimatlar [bu destek makalesinde](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)verilmiştir.</span><span class="sxs-lookup"><span data-stu-id="fa92c-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

