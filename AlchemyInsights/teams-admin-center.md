---
title: Teams Yönetim Merkezi
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
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670384"
---
# <a name="teams-admin-center"></a><span data-ttu-id="84234-102">Teams Yönetim Merkezi</span><span class="sxs-lookup"><span data-stu-id="84234-102">Teams Admin Center</span></span>

<span data-ttu-id="84234-103">[Teams Yönetim Merkezi](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center) ile Teams’i yönetmeyi öğrenin.</span><span class="sxs-lookup"><span data-stu-id="84234-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="84234-104">Teams Yönetim Merkezi’ne erişemiyorsanız lütfen aşağıdaki öğeleri denetleyin:</span><span class="sxs-lookup"><span data-stu-id="84234-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="84234-105">Tüm çevre cihazlarında (güvenlik duvarı gibi) veya yerel makinenizdeki güvenlik duvarı kurallarında uygun [Office 365 IP adreslerine ve URL'lerine](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) izin verdiğinizi doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="84234-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="84234-106">Teams Yönetim Portalı’na erişirken kullandığınız oturum açma bilgilerinin [Microsoft 365 Yönetim portalında](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) listelenen kullanıcı adınızla eşleştiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="84234-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="84234-107">Teams Yönetim Merkezi’nde kullanıcılar gösterilmiyorsa aşağıdakileri denetleyin:</span><span class="sxs-lookup"><span data-stu-id="84234-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="84234-108">Son 24 saat içinde kullanıcı oluşturdunuz veya lisans atadınız mı?</span><span class="sxs-lookup"><span data-stu-id="84234-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="84234-109">Destek bileti açmadan önce lütfen en az 24 saat beklediğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="84234-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="84234-110">Uygun lisansları atadığınızı doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="84234-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="84234-111">Şirket içi bir Active Directory 'niz varsa, [yerel Active Directory 'Nizde proxyAddresses alanında msRTCSIP-primaryuseradresinin veya SIP adresinin değerinin benzersiz olduğunu ve biçimin](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) , [Microsoft 365 Yönetim Merkezi](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)'nde kullanıcının**adı** ile eşleştiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="84234-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="84234-112">Skype Kurumsal sunucu dağıtımını korumak ve kullanıcıların şirket içi ve çevrimiçi şirket içinde olmasını istiyorsanız: Skype Kurumsal sunucusu denetim masasında **"ekiplerle kurumsal ve Skype Kurumsal Çevrimiçi**</span><span class="sxs-lookup"><span data-stu-id="84234-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
