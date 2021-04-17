---
title: Teams Yönetim Merkezi
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
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826399"
---
# <a name="teams-admin-center"></a><span data-ttu-id="7d8af-102">Teams Yönetim Merkezi</span><span class="sxs-lookup"><span data-stu-id="7d8af-102">Teams Admin Center</span></span>

<span data-ttu-id="7d8af-103">[Teams Yönetim Merkezi](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center) ile Teams’i yönetmeyi öğrenin.</span><span class="sxs-lookup"><span data-stu-id="7d8af-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="7d8af-104">Teams Yönetim Merkezi’ne erişemiyorsanız lütfen aşağıdaki öğeleri denetleyin:</span><span class="sxs-lookup"><span data-stu-id="7d8af-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="7d8af-105">Tüm çevre cihazlarında (güvenlik duvarı gibi) veya yerel makinenizdeki güvenlik duvarı kurallarında uygun [Office 365 IP adreslerine ve URL'lerine](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) izin verdiğinizi doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="7d8af-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="7d8af-106">Teams Yönetim Portalı’na erişirken kullandığınız oturum açma bilgilerinin [Microsoft 365 Yönetim portalında](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) listelenen kullanıcı adınızla eşleştiğini doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="7d8af-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="7d8af-107">Teams Yönetim Merkezi’nde kullanıcılar gösterilmiyorsa aşağıdakileri denetleyin:</span><span class="sxs-lookup"><span data-stu-id="7d8af-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="7d8af-108">Son 24 saat içinde kullanıcı oluşturdunuz veya lisans atadınız mı?</span><span class="sxs-lookup"><span data-stu-id="7d8af-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="7d8af-109">Destek bileti açmadan önce lütfen en az 24 saat beklediğinizden emin olun.</span><span class="sxs-lookup"><span data-stu-id="7d8af-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="7d8af-110">Uygun lisansları atadığınızı doğrulayın.</span><span class="sxs-lookup"><span data-stu-id="7d8af-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="7d8af-111">Şirket içi Active Directory'niz varsa, yerel Active Directory'nizin [ProxyAddresses alanında msRTCSIP-PrimaryUserAddress veya SIP](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) adresinin değerinin benzersiz olduğunu ve sip biçimiyle eş şifresinin olduğunu **doğrulayın:** [Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)yönetim merkezinden kullanıcının kullanıcı adı.</span><span class="sxs-lookup"><span data-stu-id="7d8af-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="7d8af-112">Skype Kurumsal Sunucu dağıtımını tutmak ve kullanıcıların şirket içinde ve Çevrimiçi sürümde oturum sahibi olacak şekilde sahip olmak için: Skype Kurumsal Sunucu Denetim Masası'nda "Teams ve Skype Kurumsal Çevrimiçi Sürüm ile karma **kurulum"** yönergelerini izleyin ve kullanıcıları Çevrimiçi olarak hareket ettirin.</span><span class="sxs-lookup"><span data-stu-id="7d8af-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
