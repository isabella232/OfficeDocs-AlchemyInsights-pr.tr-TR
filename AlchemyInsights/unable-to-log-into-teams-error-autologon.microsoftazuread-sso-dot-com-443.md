---
title: autologon.microsoftazuread-sso.com:443 Hatası nedeniyle Teams’te oturum açılamadı
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932285"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="273a4-102">autologon.microsoftazuread-sso dot com:443 Hatası nedeniyle Teams’te oturum açılamadı</span><span class="sxs-lookup"><span data-stu-id="273a4-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="273a4-103">O365 kimlik doğrulaması olarak Sorunsuz SSO etkinleştirildiyse, "autologon.microsoftazuread-sso.com URL’sinin Intranet Siteleri’ne eklenmesi gerelebilir.</span><span class="sxs-lookup"><span data-stu-id="273a4-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="273a4-104">Daha önce Güvenilen Siteler’e eklendiyse ve Sorunsuz SSO kullanılıyorsa, Güvenilen Siteler’den kaldırılmalıdır.</span><span class="sxs-lookup"><span data-stu-id="273a4-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="273a4-105">Lütfen [Sorunsuz SSO Sorun Giderme Denetim Listesi](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist) başlığını inceleyin.</span><span class="sxs-lookup"><span data-stu-id="273a4-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="273a4-106">Intranet Siteleri listesine URL eklemek için bu adımları izleyin:</span><span class="sxs-lookup"><span data-stu-id="273a4-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="273a4-107">**Başlat** düğmesine tıklayarak Internet Explorer’ı açın.</span><span class="sxs-lookup"><span data-stu-id="273a4-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="273a4-108">Arama kutusuna Internet Explorer yazın ve sonuç listesinde **Internet Explorer**’a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="273a4-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="273a4-109">**Araçlar**’a tıklayın ve ardından **İnternet seçenekleri**’ne tıklayın.</span><span class="sxs-lookup"><span data-stu-id="273a4-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="273a4-110">**Güvenlik** sekmesine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="273a4-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="273a4-111">Şimdi, **Lerel Intranet Siteleri**’ne ve ardından **Siteler** düğmesine tıklayın ve sonra da **Gelişmiş** düğmesine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="273a4-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="273a4-112">Web sitesi URL’sini girin ve **Ekle**’ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="273a4-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="273a4-113">Bitirdiğinizde **Kaydet**'e tıklayın.</span><span class="sxs-lookup"><span data-stu-id="273a4-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="273a4-114">Daha fazla bilgi edinmek için bkz. [O365 için Kesintisiz SSO’yu dağıtma Belgeleri](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (3. adımda Intranet Sitelerine bir URL eklemek için İlke tabanlı bir işlem içerir).</span><span class="sxs-lookup"><span data-stu-id="273a4-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
