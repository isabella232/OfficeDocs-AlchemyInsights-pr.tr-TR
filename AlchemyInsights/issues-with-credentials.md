---
title: Kimlik bilgileriyle ilgili sorunlar
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063722"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="f2b41-102">Kimlik bilgileriyle ilgili sorunlar</span><span class="sxs-lookup"><span data-stu-id="f2b41-102">Issues with credentials</span></span>

<span data-ttu-id="f2b41-103">[Microsoft kimlik platformu ve OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) istemci kimlik bilgileri akışı, doğrudan OAuth 2.0 istemci kimlik bilgileri erişim akışına karşı nasıl programlanacaklarını açıklar.</span><span class="sxs-lookup"><span data-stu-id="f2b41-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="f2b41-104">**Uygulamanın parolasını veya sertifika kimlik bilgilerini nasıl yönetirim?**</span><span class="sxs-lookup"><span data-stu-id="f2b41-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="f2b41-105">Azure CLI'de, bir [uygulamanın parolasını veya](https://docs.microsoft.com/cli/azure/ad/app/credential) sertifika kimlik bilgilerini silmek, listele veya sıfırlamak için az ad uygulaması kimlik bilgilerini kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="f2b41-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="f2b41-106">**Kullanıcılarım parolalarını nasıl sıfırlar?**</span><span class="sxs-lookup"><span data-stu-id="f2b41-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="f2b41-107">Kullanıcıların [parolalarını sıfırlayamadan önce self](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) servis parola sıfırlama için kaydolmaları gerekir.</span><span class="sxs-lookup"><span data-stu-id="f2b41-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="f2b41-108">Kullanıcı kayıt olduktan sonra bu makaledeki yönergeleri izleyerek parolasını sıfırlayabilirsiniz: [İş veya okul parolanızı sıfırlayın.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="f2b41-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="f2b41-109">**Kullanıcılarım parolalarını nasıl değiştirir?**</span><span class="sxs-lookup"><span data-stu-id="f2b41-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="f2b41-110">Kullanıcılar bu makaledeki adımları kullanarak parolalarını değiştirebilir: [Parolanızı değiştirme.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="f2b41-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="f2b41-111">Ayrıca, iki [aşamalı doğrulama için uygulama parolalarını da yönetebilirler.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="f2b41-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="f2b41-112">**Kullanıcım parolasını değiştirirken veya sıfırlarken hata alıyor**</span><span class="sxs-lookup"><span data-stu-id="f2b41-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="f2b41-113">Bu bağlantı, kullanıcı parolasını sıfırlamaya çalışırken ortaya çıkabilecek yaygın sorunlar hakkında bilgi sağlar: Sık karşılaşılan [sorunlar ve onların çözümleri](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="f2b41-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="f2b41-114">**Kullanıcının parolasını sıfırlamayla ilgili bir sorun var**</span><span class="sxs-lookup"><span data-stu-id="f2b41-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="f2b41-115">Parolaları sıfırlama yetkiniz olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="f2b41-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="f2b41-116">*Kullanıcı parolalarını yalnızca genel parolalar ve kullanıcı yöneticileri sıfırlar.*</span><span class="sxs-lookup"><span data-stu-id="f2b41-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="f2b41-117">Genel yöneticiler, diğer ayrıcalıklı yönetici parolalarını da sıfırlar.</span><span class="sxs-lookup"><span data-stu-id="f2b41-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="f2b41-118">Lisans gereksinimlerini anlayalın:</span><span class="sxs-lookup"><span data-stu-id="f2b41-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="f2b41-119">Kuruluşta en az bir lisans atanmış olması gerekir:</span><span class="sxs-lookup"><span data-stu-id="f2b41-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="f2b41-120">**Yalnızca bulut kullanıcıları** - Ücretli tüm Office 365 (O365) SKU'ları veya Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="f2b41-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="f2b41-121">**Bulut ve/veya şirket içi** kullanıcılar - Azure AD Premium P1 veya P2, Enterprise Mobility + Security (EMS) veya Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="f2b41-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="f2b41-122">Lisans gereksinimleri hakkında daha fazla bilgi edinmek için, Azure AD self servis parola sıfırlama [lisans gereksinimlerine bakın.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="f2b41-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="f2b41-123">Kullanıcının parolasını sıfırlamak için, Azure AD'de bir kullanıcı bulun.</span><span class="sxs-lookup"><span data-stu-id="f2b41-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="f2b41-124">Ardından, söz alan kullanıcıya genel bakış blade'inde "parolayı sıfırla" düğmesine tıklayın.</span><span class="sxs-lookup"><span data-stu-id="f2b41-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="f2b41-125">**Parola sıfırlama düğmesi gri**</span><span class="sxs-lookup"><span data-stu-id="f2b41-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="f2b41-126">Bu kullanıcının parolalarını **sıfırlama yetkiniz** yok.</span><span class="sxs-lookup"><span data-stu-id="f2b41-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="f2b41-127">*Kullanıcı parolalarını yalnızca genel parolalar ve kullanıcı yöneticileri sıfırlar.*</span><span class="sxs-lookup"><span data-stu-id="f2b41-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="f2b41-128">Genel yöneticiler, diğer ayrıcalıklı yönetici parolalarını da sıfırlar.</span><span class="sxs-lookup"><span data-stu-id="f2b41-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="f2b41-129">**Parola sıfırlama blade'ini göremiyorum**</span><span class="sxs-lookup"><span data-stu-id="f2b41-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="f2b41-130">Parolaları sıfırlama yetkiniz yok.</span><span class="sxs-lookup"><span data-stu-id="f2b41-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="f2b41-131">*Kullanıcı parolalarını yalnızca genel parolalar ve kullanıcı yöneticileri sıfırlar.*</span><span class="sxs-lookup"><span data-stu-id="f2b41-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="f2b41-132">Genel yöneticiler, diğer ayrıcalıklı yönetici parolalarını da sıfırlar.</span><span class="sxs-lookup"><span data-stu-id="f2b41-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="f2b41-133">**Parola sıfırlamada şirket içi tümleştirme blade'ini göremiyorum**</span><span class="sxs-lookup"><span data-stu-id="f2b41-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="f2b41-134">Şirket içi tümleştirme blade yalnızca karma ortamlarda görüntülenir; yani şirket içi kullanıcının parolalarını işlemek için parola geri yazma kullanıyor olursanız.</span><span class="sxs-lookup"><span data-stu-id="f2b41-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="f2b41-135">Şu durumda bu blade'i görmüyorsanız:</span><span class="sxs-lookup"><span data-stu-id="f2b41-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="f2b41-136">Parola geri yazma kullanasınız</span><span class="sxs-lookup"><span data-stu-id="f2b41-136">You are not using password writeback</span></span>
  - <span data-ttu-id="f2b41-137">Parola geri yazma işleminin yükleme/bağlantısı ile ilgili bir sorun var</span><span class="sxs-lookup"><span data-stu-id="f2b41-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="f2b41-138">Azure AD Connect'in yükleme/bağlantısı ile ilgili bir sorun var</span><span class="sxs-lookup"><span data-stu-id="f2b41-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="f2b41-139">Parola geri yazma ile ilgili sorunlar için daha fazla sorun giderme adımı için bkz. [Parola geri yazma sorunlarını giderme](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="f2b41-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="f2b41-140">**Bir kullanıcının parolasını nasıl sıfırlay bilmiyorum**</span><span class="sxs-lookup"><span data-stu-id="f2b41-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="f2b41-141">Uygun bir yönetici olarak Azure portalında oturum açın.</span><span class="sxs-lookup"><span data-stu-id="f2b41-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="f2b41-142">Kullanıcılar ve gruplar **blade'ine gidin,** Tüm **Kullanıcılar'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="f2b41-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="f2b41-143">Listeden bir kullanıcı seçin.</span><span class="sxs-lookup"><span data-stu-id="f2b41-143">Select a user from the list.</span></span>
4. <span data-ttu-id="f2b41-144">Seçili kullanıcı için Genel **Bakış'ı seçin** ve sonra komut çubuğunda Parolayı **sıfırla'yı seçin.**</span><span class="sxs-lookup"><span data-stu-id="f2b41-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="f2b41-145">Parolayı **sıfırla** düğmesini seçin ve ekrandaki yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="f2b41-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="f2b41-146">Yalnızca Azure portal desteği ile **gerçekleştirilen sıfırlamalar** parola geri yazma işlemidir.</span><span class="sxs-lookup"><span data-stu-id="f2b41-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="f2b41-147">**Şirket içi kullanıcı parolasını Office 365 Yönetim portalında veya Office 365 mobil uygulamasından sıfırlayam, ancak kullanıcı yine de oturum ala**</span><span class="sxs-lookup"><span data-stu-id="f2b41-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="f2b41-148">Parola Geri Yazma bu portalda desteklenmiyor.</span><span class="sxs-lookup"><span data-stu-id="f2b41-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="f2b41-149">Azure portalda kullanıcının parolasını yeniden sıfırlayın.</span><span class="sxs-lookup"><span data-stu-id="f2b41-149">Reset the user's password again in the Azure portal.</span></span>
