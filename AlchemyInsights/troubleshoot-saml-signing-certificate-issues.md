---
title: SAML imzalama sertifikası sorunlarını giderme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694453"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="a3b20-102">SAML imzalama sertifika sorunlarını giderme</span><span class="sxs-lookup"><span data-stu-id="a3b20-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="a3b20-103">SAML İmzalama sertifika sorununu çözmek için, aşağıdaki önerilen adımları uygulayın:</span><span class="sxs-lookup"><span data-stu-id="a3b20-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="a3b20-104">SSO'u destekleyen bir kurumsal uygulama eklerken Azure, SAML İmzalama sertifikası olarak adlandırılan [bir sertifika üretir.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)</span><span class="sxs-lookup"><span data-stu-id="a3b20-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="a3b20-105">Bu sertifikanın son kullanma tarihi 3 yıldır.</span><span class="sxs-lookup"><span data-stu-id="a3b20-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="a3b20-106">Sertifikanın son kullanma tarihini değiştirmek için bkz. Federasyon sertifikanız için son kullanma tarihini özelleştirme ve yeni [bir sertifikaya teslim edin.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)</span><span class="sxs-lookup"><span data-stu-id="a3b20-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="a3b20-107">Azure, uygulama tarafından istenen SAML belirteçlerini imzalamak ve başarılı bir SSO için bu sertifikayı uygulamaya göndermek için kullanır.</span><span class="sxs-lookup"><span data-stu-id="a3b20-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="a3b20-108">Bunun tamamlanması için Azure portaldan sertifikayı indirin ve SSO işlemini tamamlamak için uygulama satıcısına gönderin.</span><span class="sxs-lookup"><span data-stu-id="a3b20-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="a3b20-109">Bu işlem tamamlandıktan sonra, uygulama bu sertifikaya güvenir ve bu sertifikayla imzalanan tüm SAML belirteçleri uygulama tarafından kabul edilir.</span><span class="sxs-lookup"><span data-stu-id="a3b20-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="a3b20-110">Bu sertifikanın süresi dolsa, yeni bir sertifika oluşturun, bunu uygulama satıcısına güncelleştirin ve Azure tarafında etkin hale kurun.</span><span class="sxs-lookup"><span data-stu-id="a3b20-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="a3b20-111">Daha fazla bilgi için [bkz. Süresi yakında dolacak olan bir sertifikayı yenileme.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)</span><span class="sxs-lookup"><span data-stu-id="a3b20-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="a3b20-112">Sertifikanın süresi dolsa, kullanıcı engellanmaz.</span><span class="sxs-lookup"><span data-stu-id="a3b20-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="a3b20-113">[Geçerli sertifikanın süresi dolmadan önce](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) bildirimleri almak için bir e-posta adresi ekleyin.</span><span class="sxs-lookup"><span data-stu-id="a3b20-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="a3b20-114">4. Adım isteğe bağlı bir adımdır.</span><span class="sxs-lookup"><span data-stu-id="a3b20-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="a3b20-115">Bir uygulamanın SAML sertifika imzalama seçeneklerini ve sertifika imzalama algoritmasını değiştirebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="a3b20-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="a3b20-116">Daha fazla bilgi için [bkz. Sertifika imzalama seçeneklerini ve imzalama algoritmasını değiştirme.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="a3b20-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

