---
title: Modern Azure e-posta faturalaması
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
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820846"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="17379-102">Azure'da e-posta faturalama</span><span class="sxs-lookup"><span data-stu-id="17379-102">Email invoicing in Azure</span></span>

<span data-ttu-id="17379-103">E-posta fatura tercihini güncelleştirmek için, faturalandırma profilinde veya fatura hesabında bir sahibi veya katkıda bulunan rolüne sahip olmak gerekir.</span><span class="sxs-lookup"><span data-stu-id="17379-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="17379-104">Kabul ettiyseniz, fatura profilinde sahibi, katkıda bulunan, okuyucu ve fatura yöneticisi rolü olan tüm kullanıcılar faturasını e-postayla alır.</span><span class="sxs-lookup"><span data-stu-id="17379-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="17379-105">[Azure portalında oturum açın.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="17379-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="17379-106">**Maliyet Yönetimi + Faturalama** için arama yapın.</span><span class="sxs-lookup"><span data-stu-id="17379-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="17379-107">Sol **taraftan Faturalar'ı** seçin ve sonra sayfanın üst **kısmından Faturayı** E-posta Olarak Gönder'i seçin.</span><span class="sxs-lookup"><span data-stu-id="17379-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="17379-108">Birden fazla ödeme profiliniz varsa bir fatura profili seçin ve sonra da **Kabul'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="17379-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="17379-109">**Güncelleştir'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="17379-109">Select **Update**.</span></span>
6. <span data-ttu-id="17379-110">Birden fazla ödeme profiliniz varsa bir fatura profili seçin ve sonra da **Kabul'i seçin.**</span><span class="sxs-lookup"><span data-stu-id="17379-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="17379-111">Diğer kullanıcılara, bir MCA veya MPA faturalama profili için fatura yöneticisi rolü ataarak faturaları görüntüleme, indirme ve ödeme izni ve verme izni ve vermeksiniz.</span><span class="sxs-lookup"><span data-stu-id="17379-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="17379-112">Faturanızı e-postayla almayı tercih ettiysanız, kullanıcılar faturaları e-postayla da alır.</span><span class="sxs-lookup"><span data-stu-id="17379-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="17379-113">[Azure portalında oturum açın.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="17379-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="17379-114">**Maliyet Yönetimi + Faturalama** için arama yapın.</span><span class="sxs-lookup"><span data-stu-id="17379-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="17379-115">Sol **taraftan Fatura** profilleri'ne tıklayın.</span><span class="sxs-lookup"><span data-stu-id="17379-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="17379-116">Fatura profilleri listesinde, fatura yöneticisi rolü atamak istediğiniz fatura profilini seçin.</span><span class="sxs-lookup"><span data-stu-id="17379-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="17379-117">Sol **taraftan Erişim Denetimi (IAM)** öğesini seçin ve sonra da sayfanın üst kısmından Ekle'yi seçin. </span><span class="sxs-lookup"><span data-stu-id="17379-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="17379-118">Rol açılan listesinde Fatura **Yöneticisi'ni seçin.**</span><span class="sxs-lookup"><span data-stu-id="17379-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="17379-119">Erişim vermek için kullanıcının e-posta adresini girin.</span><span class="sxs-lookup"><span data-stu-id="17379-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="17379-120">Rolü **atamak** için Kaydet'i seçin.</span><span class="sxs-lookup"><span data-stu-id="17379-120">Select **Save** to assign the role.</span></span>
