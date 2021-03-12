---
title: Ağ iletisi kimliğini sağlayarak e-posta iletisi gönderme
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748205"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="64942-102">Ağ iletisi kimliğini sağlayarak e-posta iletisi gönderme</span><span class="sxs-lookup"><span data-stu-id="64942-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="64942-103">Yeni gönderim **uç bilgisinde,** E-posta **ve Ağ** **İletiSi Kimliği'ne seçin.**</span><span class="sxs-lookup"><span data-stu-id="64942-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="64942-104">Outlook'ta e-posta iletisi için ileti kimliğini bulmak için şu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="64942-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="64942-105">E-posta iletisine çift tıklayın ve açın.</span><span class="sxs-lookup"><span data-stu-id="64942-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="64942-106">Dosya **Özellikleri'ne**  >  **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="64942-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="64942-107">Not Defteri'ni veya boş bir Word belgesini açın ve görünürlüğü artırmak için **İnternet** üst bilgileri kutusunda bulunan içeriği kopyalayıp açık belgeye yapıştırın.</span><span class="sxs-lookup"><span data-stu-id="64942-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="64942-108">**X-MS-Exchange-Organization-Network-Message-Id alanını** bulun.</span><span class="sxs-lookup"><span data-stu-id="64942-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="64942-109">Bundan sonra gelen **değer:** gönderiniz için gereken kimliktir.</span><span class="sxs-lookup"><span data-stu-id="64942-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="64942-110">Alıcılar **altında,** e-posta bu e-postanın tüm alıcıları için gereksiz posta klasörüne inerse, **Seç'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="64942-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="64942-111">Yoksa, yalnızca sorunu bildiren kullanıcıyı seçin.</span><span class="sxs-lookup"><span data-stu-id="64942-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="64942-112">Gönderme **nedeni altında,** Engellenmiş olmalı seçeneğini belirtir, iletinin İstenmeyen **Posta,** Kimlik Avı veya Kötü Amaçlı Yazılım olarak engellenmiş olup olmadığını belirtin ve gönder'i **seçin.**  </span><span class="sxs-lookup"><span data-stu-id="64942-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="64942-113">Daha fazla bilgi edinmek için [bkz. Tarama için şüpheli istenmeyen posta, kimlik avı, URL'ler ve dosyaları Microsoft'a gönderme.](https://go.microsoft.com/fwlink/?linkid=2101479)</span><span class="sxs-lookup"><span data-stu-id="64942-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
