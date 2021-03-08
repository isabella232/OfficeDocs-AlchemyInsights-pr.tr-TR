---
title: Office 365 Güvenlik ve Uyumluluk Merkezi'nde Denetim & atama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527556"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="9ddd4-102">Office 365 Güvenlik ve Uyumluluk Merkezi'nde Denetim & atama</span><span class="sxs-lookup"><span data-stu-id="9ddd4-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="9ddd4-103">Office 365 denetim günlüğünde arama yapmak için,  bir yöneticiye Exchange Online'da Yalnızca Görüntüleme Denetim Günlükleri rolü veya **Denetim** Günlükleri rolü atanabilir.</span><span class="sxs-lookup"><span data-stu-id="9ddd4-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="9ddd4-104">Bu roller varsayılan olarak Uyumluluk Yönetimi ve Kuruluş Yönetimi rol gruplarına atanır.</span><span class="sxs-lookup"><span data-stu-id="9ddd4-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="9ddd4-105">Office 365 ve Microsoft 365'te genel yöneticiler otomatik olarak Kuruluş Yönetimi rol grubunun üyeleri olarak eklenir.</span><span class="sxs-lookup"><span data-stu-id="9ddd4-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="9ddd4-106">Kullanıcının en düşük düzeydeki ayrıcalıklarla aramasine olanak sağlamak için, Exchange  Online'da özel bir  rol grubu oluşturun, Yalnızca Görüntüleme Denetim Günlükleri rolünü veya Denetim Günlükleri rolünü ekleyin ve sonra da kullanıcıyı yeni rol grubunun bir üyesi olarak ekleyin.</span><span class="sxs-lookup"><span data-stu-id="9ddd4-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="9ddd4-107">Daha fazla bilgi için, [Exchange Online'da](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) rol gruplarını yönetme ve Güvenlik ve Uyumluluk [Merkezi'nde denetim & arama yapın.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="9ddd4-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>