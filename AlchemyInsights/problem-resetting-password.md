---
title: Parola sıfırlama sorunu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696281"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="992b5-102">Parola sıfırlama sorunları</span><span class="sxs-lookup"><span data-stu-id="992b5-102">Problems resetting password</span></span>

<span data-ttu-id="992b5-103">Parolayı sıfırlarken karşılaş olabileceğiniz sorunlardan bazıları ve olası çözümler aşağıda ve aşağıda ve listelerde yer alan bazı sorunlar yermektedir:</span><span class="sxs-lookup"><span data-stu-id="992b5-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="992b5-104">**Parola sıfırlama ile ilgili diğer kategorilerde yer alan bir sorun var**</span><span class="sxs-lookup"><span data-stu-id="992b5-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="992b5-105">Parolaları sıfırlama yetkiniz olduğundan emin olun.</span><span class="sxs-lookup"><span data-stu-id="992b5-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="992b5-106">Kullanıcı parolalarını yalnızca genel parolalar ve kullanıcı yöneticileri sıfırlar.</span><span class="sxs-lookup"><span data-stu-id="992b5-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="992b5-107">Genel yöneticiler, diğer ayrıcalıklı yönetici parolalarını da sıfırlar.</span><span class="sxs-lookup"><span data-stu-id="992b5-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="992b5-108">Lisans gereksinimlerini anlamadan emin olun:</span><span class="sxs-lookup"><span data-stu-id="992b5-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="992b5-109">Kuruluşta en az bir lisans atanmış olması gerekir</span><span class="sxs-lookup"><span data-stu-id="992b5-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="992b5-110">Yalnızca bulut kullanıcıları - Ücretli tüm Office 365 (O365) SKU'ları veya Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="992b5-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="992b5-111">Bulut ve/veya şirket içi kullanıcılar - Azure AD Premium P1 veya P2, Enterprise Mobility + Security (EMS) veya Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="992b5-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="992b5-112">Lisans gereksinimleri hakkında daha fazla bilgi için, Azure AD self servis parola sıfırlama lisans [gereksinimleri makalesine bakın.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="992b5-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="992b5-113">**Parola sıfırlama ilkemi test etmede sorunm var**</span><span class="sxs-lookup"><span data-stu-id="992b5-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="992b5-114">Son uygulanan ilkelerin tüm veri merkezlerine ve uç noktalara çoğaltılması birkaç dakika sürebilir.</span><span class="sxs-lookup"><span data-stu-id="992b5-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="992b5-115">Veri merkezinden fiziksel uzaklık da değişikliklerin ne kadar hızlı uygulandığını etkiler.</span><span class="sxs-lookup"><span data-stu-id="992b5-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="992b5-116">Küçük bir kullanıcı kümesiyle yönetici değil son kullanıcıyla test ve pilot uygulama.</span><span class="sxs-lookup"><span data-stu-id="992b5-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="992b5-117">Azure portalında yapılandırılan ilkeler yöneticilere değil YALNIZLIK son kullanıcılara uygulanır.</span><span class="sxs-lookup"><span data-stu-id="992b5-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="992b5-118">Microsoft, herhangi bir Azure yönetici rolü için güçlü bir varsayılan iki kapılı parola sıfırlama ilkesi zorunlur (Örnek: Genel Yönetici, Yardım Masası Yöneticisi, Parola Yöneticisi, vb.)</span><span class="sxs-lookup"><span data-stu-id="992b5-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="992b5-119">Yöneticilere yönelik [ilkeler hakkında daha fazla bilgi.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="992b5-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="992b5-120">**Parola sıfırlamayı dağıtmak istiyorum, ancak kullanıcılarımı ek güvenlik bilgilerini kaydetmelerini istemiyorum**</span><span class="sxs-lookup"><span data-stu-id="992b5-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="992b5-121">Kullanıcılarınız için verileri önceden doldurmak zorunda değil!</span><span class="sxs-lookup"><span data-stu-id="992b5-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="992b5-122">- Bir yönetici olarak, parola sıfırlamayı kuruluşa göndermeden önce kullanıcılarınız için telefon ve e-posta özelliklerini ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="992b5-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="992b5-123">Bunu API, PowerShell veya Azure AD Connect kullanarak da kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="992b5-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="992b5-124">Buradan daha fazla bilgi edinebilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="992b5-124">More information here:</span></span>
- [<span data-ttu-id="992b5-125">Kullanıcıların kaydolması gerekmeden parola sıfırlamayı dağıtma</span><span class="sxs-lookup"><span data-stu-id="992b5-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="992b5-126">Parola sıfırlama ile kullanılan veriler</span><span class="sxs-lookup"><span data-stu-id="992b5-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="992b5-127">**Parola sıfırlama düğmesi gri**</span><span class="sxs-lookup"><span data-stu-id="992b5-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="992b5-128">Bu kullanıcının parolalarını sıfırlama yetkiniz yok.</span><span class="sxs-lookup"><span data-stu-id="992b5-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="992b5-129">Kullanıcı parolalarını yalnızca genel parolalar ve kullanıcı yöneticileri sıfırlar.</span><span class="sxs-lookup"><span data-stu-id="992b5-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="992b5-130">Genel yöneticiler, diğer ayrıcalıklı yönetici parolalarını da sıfırlar.</span><span class="sxs-lookup"><span data-stu-id="992b5-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="992b5-131">**Parola sıfırlama blade'ini göremiyorum**</span><span class="sxs-lookup"><span data-stu-id="992b5-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="992b5-132">Parolaları sıfırlama yetkiniz yok.</span><span class="sxs-lookup"><span data-stu-id="992b5-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="992b5-133">Kullanıcı parolalarını yalnızca genel parolalar ve kullanıcı yöneticileri sıfırlar.</span><span class="sxs-lookup"><span data-stu-id="992b5-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="992b5-134">Genel yöneticiler, diğer ayrıcalıklı yönetici parolalarını da sıfırlar.</span><span class="sxs-lookup"><span data-stu-id="992b5-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="992b5-135">**Parola sıfırlamada şirket içi tümleştirme blade'ini göremiyorum**</span><span class="sxs-lookup"><span data-stu-id="992b5-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="992b5-136">Şirket içi tümleştirme blade yalnızca karma ortamlarda görüntülenir; yani şirket içi kullanıcının parolalarını işlemek için parola geri yazma kullanıyor olursanız.</span><span class="sxs-lookup"><span data-stu-id="992b5-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="992b5-137">Şu durumda bu blade'i görmüyorsanız:</span><span class="sxs-lookup"><span data-stu-id="992b5-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="992b5-138">Parola geri yazma kullanasınız</span><span class="sxs-lookup"><span data-stu-id="992b5-138">You are not using password writeback</span></span>
    - <span data-ttu-id="992b5-139">Parola geri yazma işleminin yükleme/bağlantısı ile ilgili bir sorun var</span><span class="sxs-lookup"><span data-stu-id="992b5-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="992b5-140">Azure AD Connect'in yükleme/bağlantısı ile ilgili bir sorun var</span><span class="sxs-lookup"><span data-stu-id="992b5-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="992b5-141">Parola geri yazma ile ilgili sorunlar için daha fazla sorun giderme adımı için Parola geri yazma [sorunlarını giderme bölümüne bakın](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="992b5-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="992b5-142">**Bir kullanıcının parolasını nasıl sıfırlay bilmiyorum**</span><span class="sxs-lookup"><span data-stu-id="992b5-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="992b5-143">Uygun bir yönetici olarak Azure portalında oturum açın.</span><span class="sxs-lookup"><span data-stu-id="992b5-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="992b5-144">Kullanıcılar ve gruplar blade'ine gidin, Tüm **Kullanıcılar'ı seçin.**</span><span class="sxs-lookup"><span data-stu-id="992b5-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="992b5-145">Listeden bir kullanıcı seçin.</span><span class="sxs-lookup"><span data-stu-id="992b5-145">Select a user from the list.</span></span>
1. <span data-ttu-id="992b5-146">Seçili kullanıcı için Genel **Bakış'ı seçin** ve sonra komut çubuğunda Parolayı sıfırla'ya **tıklayın.**</span><span class="sxs-lookup"><span data-stu-id="992b5-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="992b5-147">Ekrandaki yönergeleri izleyin.</span><span class="sxs-lookup"><span data-stu-id="992b5-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="992b5-148">Yalnızca Azure portal desteği ile gerçekleştirilen sıfırlamalar parola geri yazma işlemidir.</span><span class="sxs-lookup"><span data-stu-id="992b5-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="992b5-149">**Şirket içi kullanıcı parolasını Office 365 Yönetim portalında veya Office 365 mobil uygulamasından sıfırlayam, ancak kullanıcı yine de oturum ala**</span><span class="sxs-lookup"><span data-stu-id="992b5-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="992b5-150">Parola Geri Yazma bu portalda desteklenmiyor.</span><span class="sxs-lookup"><span data-stu-id="992b5-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="992b5-151">Azure portalında kullanıcının parolasını yeniden sıfırlama - portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="992b5-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

