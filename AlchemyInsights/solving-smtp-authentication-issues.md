---
title: SMTP kimlik doğrulamasını ve sorun gidermeyi etkinleştirme
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077671"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="c6971-102">SMTP kimlik doğrulamasını ve sorun gidermeyi etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="c6971-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="c6971-103">Bir posta kutusu için SMTP kimlik doğrulamasını etkinleştirmek veya Microsoft 365 ile bir cihaz veya uygulamanın kimlik doğrulaması gerçekleştirerek e-posta geçişi gerçekleştirerek geçiş yapmaya çalışmanız sırasında 5.7.57 veya 5.7.3 veya 5.7.139 kodlu "İstemci kimliği doğrulanmadı", "Kimlik doğrulaması başarısız" veya "SmtpClientAuthentication" hatası alıyorsanız, sorunu çözmek için şu üç eylemi gerçekleştirin:</span><span class="sxs-lookup"><span data-stu-id="c6971-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="c6971-104">Güvenlik [varsayılanlarını hayır olarak etkinleştir'i](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) seçenek tarak Azure **güvenlik varsayılanlarını devre** dışı **bırak.**</span><span class="sxs-lookup"><span data-stu-id="c6971-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="c6971-105">a.</span><span class="sxs-lookup"><span data-stu-id="c6971-105">a.</span></span> <span data-ttu-id="c6971-106">Güvenlik yöneticisi, Koşullu Erişim yöneticisi veya genel yönetici olarak Azure portalında oturum açın.</span><span class="sxs-lookup"><span data-stu-id="c6971-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="c6971-107">b.</span><span class="sxs-lookup"><span data-stu-id="c6971-107">b.</span></span> <span data-ttu-id="c6971-108">Azure Active Directory > **göz atabilirsiniz.**</span><span class="sxs-lookup"><span data-stu-id="c6971-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="c6971-109">c.</span><span class="sxs-lookup"><span data-stu-id="c6971-109">c.</span></span> <span data-ttu-id="c6971-110">Güvenlik **varsayılanlarını yönet'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="c6971-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="c6971-111">d.</span><span class="sxs-lookup"><span data-stu-id="c6971-111">d.</span></span> <span data-ttu-id="c6971-112">Güvenlik **varsayılanlarını etkinleştir ayarını Hayır** olarak **ayarlayın.**</span><span class="sxs-lookup"><span data-stu-id="c6971-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="c6971-113">e.</span><span class="sxs-lookup"><span data-stu-id="c6971-113">e.</span></span> <span data-ttu-id="c6971-114">**Kaydet**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="c6971-114">Select **Save**.</span></span>

2. <span data-ttu-id="c6971-115">[Lisanslı posta kutusuna İstemci SMTP](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) gönderimi'ni etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="c6971-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="c6971-116">a.</span><span class="sxs-lookup"><span data-stu-id="c6971-116">a.</span></span> <span data-ttu-id="c6971-117">Arama Microsoft 365 yönetim merkezi, Etkin **Kullanıcılar'a gidin** ve kullanıcısı seçin.</span><span class="sxs-lookup"><span data-stu-id="c6971-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="c6971-118">b.</span><span class="sxs-lookup"><span data-stu-id="c6971-118">b.</span></span> <span data-ttu-id="c6971-119">Posta sekmesine gidin ve E-posta **uygulamaları'nın altında E-posta** uygulamalarını **yönet'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="c6971-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="c6971-120">d.</span><span class="sxs-lookup"><span data-stu-id="c6971-120">d.</span></span> <span data-ttu-id="c6971-121">Kimliği Doğrulanmış **SMTP'nin işaretli** olduğundan (etkinleştirildiğinden) emin olun.</span><span class="sxs-lookup"><span data-stu-id="c6971-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="c6971-122">e.</span><span class="sxs-lookup"><span data-stu-id="c6971-122">e.</span></span> <span data-ttu-id="c6971-123">Değişiklikleri **kaydet'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="c6971-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="c6971-124">[Lisanslı posta kutusunda Multi-Factor Authentication'ı (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) devre dışı bırakma.</span><span class="sxs-lookup"><span data-stu-id="c6971-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="c6971-125">a.</span><span class="sxs-lookup"><span data-stu-id="c6971-125">a.</span></span> <span data-ttu-id="c6971-126">Gezinti Bölmesi'Microsoft 365 yönetim merkezi ve sol gezinti menüsünde Kullanıcılar Etkin **Kullanıcılar'ı**  >  **seçin.**</span><span class="sxs-lookup"><span data-stu-id="c6971-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="c6971-127">b.</span><span class="sxs-lookup"><span data-stu-id="c6971-127">b.</span></span> <span data-ttu-id="c6971-128">**Multi-factor authentication öğesini seçin.**</span><span class="sxs-lookup"><span data-stu-id="c6971-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="c6971-129">c.</span><span class="sxs-lookup"><span data-stu-id="c6971-129">c.</span></span> <span data-ttu-id="c6971-130">Kullanıcıyı seçin ve **Multi-Factorauth özelliğini devre dışı bırakma.**</span><span class="sxs-lookup"><span data-stu-id="c6971-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
