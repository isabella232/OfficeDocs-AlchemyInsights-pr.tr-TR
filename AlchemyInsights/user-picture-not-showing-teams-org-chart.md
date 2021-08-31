---
title: Kullanıcı resmi kuruluş şemasında Microsoft Teams resmi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792889"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Kullanıcı resmi kuruluş şemasında Microsoft Teams resmi

Kuruluş şemasında bir veya birden çok kişinin kuruluş şemasında profil fotoğrafı yoksa **ShowInAddressLists** ayarının **False** olarak ayarlanmış olabilir:

1. Etkin [**Microsoft 365 yönetim merkezi >'e**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)gidin ve eksik fotoğrafı olan kullanıcıyı seçin. 
1. Posta sekmesini **seçin** ve Genel adres listesinde **göster'in Evet olarak ayarlanmış** olduğundan emin **olun.** 

**ShowInAddressLists'i** **Evet** olarak ayarlama işe yaramadı ise, şunları kontrol edin:

- Kullanıcı, dosyada alıcı listesinden Exchange. Daha fazla bilgi için [bkz. Exchange Online'da adres listelerini yönetme.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- Kullanıcı, E-posta'daki adres listesinden Azure Active Directory. Daha fazla bilgi için bkz. [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
