---
title: Hizmet Bağlantı Noktasını (SCP) Yapılandırma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037292"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="98a5e-102">Hizmet bağlantı noktasını (SCP) yapılandırma</span><span class="sxs-lookup"><span data-stu-id="98a5e-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="98a5e-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="98a5e-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="98a5e-104">**Neden:** SCP nesnesi okunamıyor ve Azure AD kiracı bilgilerine ulaşamıyor</span><span class="sxs-lookup"><span data-stu-id="98a5e-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="98a5e-105">**Çözüm:** Hizmet Bağlantı Noktası [Yapılandırma bölümüne bakın](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="98a5e-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="98a5e-106">**Eylem planı**</span><span class="sxs-lookup"><span data-stu-id="98a5e-106">**Action plan**</span></span>

- <span data-ttu-id="98a5e-107">Cihazın denetimli doğrulama için GPO'ya sahip olup olmadığını kontrol edin.</span><span class="sxs-lookup"><span data-stu-id="98a5e-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="98a5e-108">GPO'nun kayıt defteri anahtarlarını oluşturduğuna emin olun.</span><span class="sxs-lookup"><span data-stu-id="98a5e-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="98a5e-109">Dizin kimliği ve onmicrosoft etki alanıyla 2 anahtar oluşturduğunuzdan emin olun.</span><span class="sxs-lookup"><span data-stu-id="98a5e-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="98a5e-110">**SCP için istemci tarafı kayıt defteri ayarını yapılandırma**</span><span class="sxs-lookup"><span data-stu-id="98a5e-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="98a5e-111">Cihazlarınızı kayıt defterinde SCP girdisini yapılandıran bir kayıt defteri ayarını dağıtmak üzere Grup İlkesi Nesnesi (GPO) oluşturmak için aşağıdaki örneği kullanın.</span><span class="sxs-lookup"><span data-stu-id="98a5e-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="98a5e-112">Grup İlkesi Yönetim konsolu açın ve etki alanınıza yeni bir GPO oluşturun.</span><span class="sxs-lookup"><span data-stu-id="98a5e-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="98a5e-113">Yeni oluşturduğunuz GPO'ya bir ad verin (örneğin, ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="98a5e-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="98a5e-114">GPO'u düzenleyin ve şu yolu bulun: Bilgisayar **Yapılandırması > Tercihleri ve Windows > Ayarları > Defteri.**</span><span class="sxs-lookup"><span data-stu-id="98a5e-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="98a5e-115">Kayıt Defteri'ne **sağ tıklayın** ve Kayıt **Defteri >'ni seçin.**</span><span class="sxs-lookup"><span data-stu-id="98a5e-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="98a5e-116">Genel **sekmesinde,** aşağıdakini yapılandırabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="98a5e-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="98a5e-117">**Eylem**: Güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="98a5e-117">**Action**: Update</span></span>
    
- <span data-ttu-id="98a5e-118">**Kurye**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="98a5e-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="98a5e-119">**Anahtar Yolu:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="98a5e-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="98a5e-120">**Değer adı**: TenantId</span><span class="sxs-lookup"><span data-stu-id="98a5e-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="98a5e-121">**Değer türü:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="98a5e-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="98a5e-122">**Değer verileri:** Azure AD örneğinizin GUID veya Dizin Kimliği (Bu değer Azure portalında > **Azure Active Directory > Özellikleri > Dizin Kimliği)**</span><span class="sxs-lookup"><span data-stu-id="98a5e-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="98a5e-123">**Tamam**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="98a5e-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="98a5e-124">Kayıt Defteri'ne **sağ tıklayın** ve Kayıt **Defteri >'ni seçin.**</span><span class="sxs-lookup"><span data-stu-id="98a5e-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="98a5e-125">Genel **sekmesinde,** aşağıdakini yapılandırabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="98a5e-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="98a5e-126">**Eylem**: Güncelleştirme</span><span class="sxs-lookup"><span data-stu-id="98a5e-126">**Action**: Update</span></span>
    
- <span data-ttu-id="98a5e-127">**Kurye**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="98a5e-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="98a5e-128">**Anahtar Yolu:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="98a5e-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="98a5e-129">**Değer adı**: TenantName</span><span class="sxs-lookup"><span data-stu-id="98a5e-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="98a5e-130">**Değer türü:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="98a5e-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="98a5e-131">**Değer verileri:** AD FS gibi bir federasyon ortamı kullanıyorsanız, doğrulanmış etki alanı adınız.</span><span class="sxs-lookup"><span data-stu-id="98a5e-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="98a5e-132">Yönetilen bir ortam kullanıyorsanız, onmicrosoft.com etki alanı adınız (örneğin, contoso.onmicrosoft).com</span><span class="sxs-lookup"><span data-stu-id="98a5e-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="98a5e-133">**Tamam**'a tıklayın.</span><span class="sxs-lookup"><span data-stu-id="98a5e-133">Click **OK**.</span></span>

7. <span data-ttu-id="98a5e-134">Yeni oluşturulan GPO için düzenleyiciyi kapatın.</span><span class="sxs-lookup"><span data-stu-id="98a5e-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="98a5e-135">Yeni oluşturulan GPO'nun bağlantısını, denetimli olarak açılan popülasyona ait etki alanına katılmış bilgisayarları içeren istenen OU'ya bın.</span><span class="sxs-lookup"><span data-stu-id="98a5e-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="98a5e-136">Daha fazla bilgi için bkz. Karma Azure AD birleştirme [denetimli doğrulaması - Azure AD | Microsoft Belgeler ve Sorun](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)  [Giderme karma Azure Active Directory'ye katılmış cihazlar ve | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="98a5e-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









