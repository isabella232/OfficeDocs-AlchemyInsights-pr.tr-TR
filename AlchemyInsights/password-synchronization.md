---
title: Parola eşitleme
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483087"
---
# <a name="password-synchronization"></a><span data-ttu-id="c65d9-102">Parola eşitleme</span><span class="sxs-lookup"><span data-stu-id="c65d9-102">Password synchronization</span></span>

<span data-ttu-id="c65d9-103">**Parola Karma Eşitlemesi hiç çalışmıyor**</span><span class="sxs-lookup"><span data-stu-id="c65d9-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="c65d9-104">Parola Karması Eşitlemesi çalışmaması sırasında müşterilerin sık karşılaştığı bazı sorunlar:</span><span class="sxs-lookup"><span data-stu-id="c65d9-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="c65d9-105">Şirket içi Active Directory ile iletişim kurmak için Azure AD Connect  tarafından kullanılan  Active Directory hesabına Dizin Değişikliklerini Çoğalt ve Dizin Değişikliklerini Çoğalt (parola eşitlemesi için gerekli olan tüm izinler) verilmmektedir. Bu izinleri Active Directory hesabına vererek bunu düzeltmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="c65d9-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="c65d9-106">Yönetici, Kullanıcı Sign-In yöntemini Parola Eşitlemesi'nden  Azure AD Connect sihirbazında **AD FS** ile Federasyon gibi başka bir seçenenle  değiştirdikten sonra parola karması eşitlemesi devre dışı bırakılır. Azure AD Connect sihirbazında parola karması eşitleme özelliğini yeniden etkinleştirerek bunu düzeltebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="c65d9-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="c65d9-107">Şirket içi Active Directory ile bağlantı sorunu.</span><span class="sxs-lookup"><span data-stu-id="c65d9-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="c65d9-108">Örneğin, bazı etki alanı denetleyicilerine Azure AD Connect [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) tarafından erişilemiyor veya gereken bağlantı noktaları Güvenlik Duvarı tarafından engellenmiş durumdadır. Azure AD Connect sunucusuyla şirket içi Active Directory arasındaki bağlantının doğru şekilde çalışmalarından emin olarak bu sorunu çözmeniz gerekir.</span><span class="sxs-lookup"><span data-stu-id="c65d9-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="c65d9-109">Azure AD Connect sunucusu şu anda hazırlama modundadır ve bu da sunucunun parola karmalarını alamamasıdır - Sorunu gidermek için, Azure AD Connect eşitlemesi ile parola eşitlemesi sorunlarını giderme bölümünde açıklanan adımları izleyin - Hiçbir parola [eşitlenmez.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="c65d9-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="c65d9-110">**Parola Karma Eşitlemesi bazı kullanıcılarım için çalışmıyor**</span><span class="sxs-lookup"><span data-stu-id="c65d9-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="c65d9-111">Parola karması kullanıcı için eşitlenemezse, sorunu  araştırmak ve çözmek için Azure AD Connect'te sorun giderme görevini kullanın.</span><span class="sxs-lookup"><span data-stu-id="c65d9-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="c65d9-112">Aşağıdaki görevleri gerçekleştirin:</span><span class="sxs-lookup"><span data-stu-id="c65d9-112">Perform the following tasks:</span></span>

    <span data-ttu-id="c65d9-113">a.</span><span class="sxs-lookup"><span data-stu-id="c65d9-113">a.</span></span> [<span data-ttu-id="c65d9-114">Sihirbazda sorun giderme görevini çalıştırma</span><span class="sxs-lookup"><span data-stu-id="c65d9-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="c65d9-115">b.</span><span class="sxs-lookup"><span data-stu-id="c65d9-115">b.</span></span> [<span data-ttu-id="c65d9-116">Belirli bir kullanım için parola karması eşitleme sorunlarını araştırmak üzere sorun giderme cmdlet'ini kullanın</span><span class="sxs-lookup"><span data-stu-id="c65d9-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="c65d9-117">Kullanıcı için şirket içi Active Directory Kullanıcı nesnesi etkinleştirildiğinde, **sonraki oturum açma seçeneğinde parolayı değiştirmesi** gerekir.</span><span class="sxs-lookup"><span data-stu-id="c65d9-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="c65d9-118">Bu seçenek etkinleştirildiğinde, kullanıcıya geçici bir parola atanır ve bir sonraki oturum açma sırasında parolayı değiştirmesi istenir.</span><span class="sxs-lookup"><span data-stu-id="c65d9-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="c65d9-119">Azure AD Connect, Geçici parolaları Azure AD'ye eşitlemez.</span><span class="sxs-lookup"><span data-stu-id="c65d9-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="c65d9-120">Yukarıdaki sorunu çözmek için, aşağıdaki görevlerden birini gerçekleştirin:</span><span class="sxs-lookup"><span data-stu-id="c65d9-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="c65d9-121">Kullanıcıdan şirket içi uygulamada (örneğin, Windows Masaüstü) oturum açmasını ve parolayı değiştirmesini iste.</span><span class="sxs-lookup"><span data-stu-id="c65d9-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="c65d9-122">Yeni parola Azure AD ile eşitlenir.</span><span class="sxs-lookup"><span data-stu-id="c65d9-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="c65d9-123">Yöneticinin, Kullanıcı'nın bir sonraki oturum açma sırasında parolasını değiştirmesi ve yeni parolayı kullanıcıyla paylaşması seçeneğini etkinleştirmeden kullanıcının parolasını güncelleştirmesini sağlamak.</span><span class="sxs-lookup"><span data-stu-id="c65d9-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="c65d9-124">Şirket içi Active Directory Kullanıcı nesnesi nesne **eşitlemesi veya** parola eşitlemesi için doğru yapılandırılmamış.</span><span class="sxs-lookup"><span data-stu-id="c65d9-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="c65d9-125">Bu sorunu gidermek için, Azure AD Connect eşitlemesi ile Parola karma eşitlemesi [sorunlarını giderme konusunda açıklanan adımları izleyin.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="c65d9-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







