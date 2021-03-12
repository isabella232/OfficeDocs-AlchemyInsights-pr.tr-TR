---
title: Office 365 için Microsoft Defender kimlik avı önleme ilkesi örneği
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750800"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="8e9b8-102">Office 365 için Microsoft Defender kimlik avı önleme ilkesi örneği</span><span class="sxs-lookup"><span data-stu-id="8e9b8-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="8e9b8-103">Bu ayarlar, Etki Alanı ve CEO olarak *adlandırılan ilkeyi etkinleştirir.*</span><span class="sxs-lookup"><span data-stu-id="8e9b8-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="8e9b8-104">Bu ilke, hem kullanıcı hem de etki alanı korumasını kimliğe bürünme karşı sağlar ve ardından bu ilkeyi etki alanı içindeki kullanıcılar tarafından alınan tüm e-postalara uygular.</span><span class="sxs-lookup"><span data-stu-id="8e9b8-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="8e9b8-105">İlk olarak, ilkeyi oluşturmak için aşağıdaki bilgileri ekleyin:</span><span class="sxs-lookup"><span data-stu-id="8e9b8-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="8e9b8-106">**Ad**: Etki alanı ve CEO **Açıklaması**: CEO'nun ve etki alanınız kimliğine bürünülmemelerini sağlar.</span><span class="sxs-lookup"><span data-stu-id="8e9b8-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="8e9b8-107">**Uygulandı:** Alıcı **etki alanını seçin.**</span><span class="sxs-lookup"><span data-stu-id="8e9b8-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="8e9b8-108">Bunların **herhangi biri altında,** **Seç'i** seçin ve sonra da bir etki alanı seçin.</span><span class="sxs-lookup"><span data-stu-id="8e9b8-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="8e9b8-109">Select **+ Add**.</span><span class="sxs-lookup"><span data-stu-id="8e9b8-109">Select **+ Add**.</span></span> <span data-ttu-id="8e9b8-110">Listede etki alanının adının yanındaki onay kutusunu seçin *(örneğin,* contoso.com) ve ardından Ekle'yi **seçin.**</span><span class="sxs-lookup"><span data-stu-id="8e9b8-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="8e9b8-111">**Bitti'yi seçin.**</span><span class="sxs-lookup"><span data-stu-id="8e9b8-111">Select **Done**.</span></span>
- <span data-ttu-id="8e9b8-112">İlke oluşturulduktan sonra, aşağıdaki seçenekleri kullanarak ilkeye ince ayar yapabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="8e9b8-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="8e9b8-113">**Korumak için kullanıcı ekleme:** Bu örnekte, CEO'nun e-posta adresini en azından ekleyin.</span><span class="sxs-lookup"><span data-stu-id="8e9b8-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="8e9b8-114">**Korumak için etki alanları ekleyin:** CEO'nun ofisini içeren kuruluş etki alanını ekleyin.</span><span class="sxs-lookup"><span data-stu-id="8e9b8-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="8e9b8-115">**Eylemleri seçin:** **E-posta** kimliğine bürünülen bir kullanıcı tarafından gönderilirse, iletiyi başka bir e-posta adresine yönlendir'i seçin ve güvenlik yöneticisinin e-posta adresini girin (örneğin, *securityadmin@contoso.com).*</span><span class="sxs-lookup"><span data-stu-id="8e9b8-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="8e9b8-116">**E-posta kimliğine bürünülen bir etki alanı tarafından gönderilirse,** **iletiyi karantinaya alın'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="8e9b8-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="8e9b8-117">**Posta kutusu** zekası: Yeni kimlik avı önleme ilkesi oluşturmanızda varsayılan olarak bu seçenek seçilidir.</span><span class="sxs-lookup"><span data-stu-id="8e9b8-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="8e9b8-118">En iyi sonuçları elde **etmek için bu** ayarı Açık bırakın.</span><span class="sxs-lookup"><span data-stu-id="8e9b8-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="8e9b8-119">**Güvenilen gönderenleri ve etki alanlarını ekleyin:** Bu örnekte, geçersiz kılmaları tanımlamayın.</span><span class="sxs-lookup"><span data-stu-id="8e9b8-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="8e9b8-120">Ayarlarınızı gözden geçirerek uygun şekilde Bu ilkeyi **oluştur veya** **Kaydet'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="8e9b8-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="8e9b8-121">Daha fazla bilgi edinmek için [Microsoft 365'te kimlik avı önleme ilkelerine bakın.](https://go.microsoft.com/fwlink/?linkid=2092235)</span><span class="sxs-lookup"><span data-stu-id="8e9b8-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
