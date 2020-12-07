---
title: Azure AD Connect'te parola geri yazmayı etkinleştirme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560460"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="3c568-102">Azure AD Connect'te parola geri yazmayı etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="3c568-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="3c568-103">Self servis parola sıfırlama geri yazmayı etkinleştirmek için önce Azure AD Connect'te geri yazma seçeneğini etkinleştirin.</span><span class="sxs-lookup"><span data-stu-id="3c568-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="3c568-104">Azure AD Connect sunucusunda aşağıdaki adımları tamamlayın:</span><span class="sxs-lookup"><span data-stu-id="3c568-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="3c568-105">Azure AD Connect sunucunuzda oturum açıp **Azure AD Connect** yapılandırma sihirbazını başlatın.</span><span class="sxs-lookup"><span data-stu-id="3c568-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="3c568-106">**Hoş Geldiniz** sayfasında, **Yapılandır**'ı tıklayın.</span><span class="sxs-lookup"><span data-stu-id="3c568-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="3c568-107">**Ek görevler** sayfasında **Eşitleme seçeneklerini özelleştir**'i seçin ve ardından **İleri**'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="3c568-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="3c568-108">**Azure AD'ye Bağlanma** sayfasında Azure kiracınız için genel yönetici kimlik bilgisi girin ve ardından **İleri**'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="3c568-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="3c568-109">**Dizinlere bağlanma** ve **Etki Alanı/OU** filtreleme sayfalarında **İleri**'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="3c568-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="3c568-110">**İsteğe bağlı özellikler** sayfasında **Parola geri yazma**'nın yanında bulunan kutuyu seçin ve **İleri**'ye tıklayın.</span><span class="sxs-lookup"><span data-stu-id="3c568-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="3c568-111">**Yapılandırmaya hazır** sayfasında **Yapılandır**'a tıklayıp işlemin bitmesini bekleyin.</span><span class="sxs-lookup"><span data-stu-id="3c568-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="3c568-112">Yapılandırmanın bittiğini gördüğünüzde **Çıkış**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="3c568-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="3c568-113">Azure AD Connect'te parola geri yazma etkinleştirildiğinde, geri yazma için Azure AD SSPR'yi yapılandırın.</span><span class="sxs-lookup"><span data-stu-id="3c568-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="3c568-114">SSPR'de parola geri yazmayı etkinleştirmek için aşağıdaki adımları tamamlayın:</span><span class="sxs-lookup"><span data-stu-id="3c568-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="3c568-115">Genel yönetici hesabınızı kullanarak Azure portal'da oturum açın.</span><span class="sxs-lookup"><span data-stu-id="3c568-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="3c568-116">**Azure Active Directory**'yi arayıp seçin, **Parolayı sıfırla**'yı tıklayın, ardından **Şirket İçi tümleştirme**'yi tıklayın.</span><span class="sxs-lookup"><span data-stu-id="3c568-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="3c568-117">**Şirket içi dizininizde parola geri yazılsın mı?** seçeneğini **Evet** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="3c568-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="3c568-118">**Kullanıcıların, parolalarını sıfırlamadan hesaplarının kilidini açmasına izin verilsin mi?** seçeneğini **Evet** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="3c568-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="3c568-119">Hazır olduğunuzda **Kaydet**’i tıklayın.</span><span class="sxs-lookup"><span data-stu-id="3c568-119">When ready, click **Save**.</span></span>

<span data-ttu-id="3c568-120">Daha fazla bilgi için bkz. [Şirket içi bir ortama Azure Active Directory self servis parola sıfırlama geri yazma özelliğini etkinleştirme.](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="3c568-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="3c568-121">Yönetici, Azure Portal'da bir kullanıcının parolasını sıfırladığında, kullanıcı şirket dışındansa veya parola karması eşitlenmişse, parola şirket içi bir ortama geri yazılır.</span><span class="sxs-lookup"><span data-stu-id="3c568-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="3c568-122">Bu işlev şu anda Office Yönetici portalında desteklenmemektedir.</span><span class="sxs-lookup"><span data-stu-id="3c568-122">This functionality is currently not supported in the Office Admin portal.</span></span>