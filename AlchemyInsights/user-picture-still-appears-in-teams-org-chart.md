---
title: Kullanıcı resmi kuruluş şemasında Microsoft Teams görünür
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422315"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Kullanıcı resmi kuruluş şemasında Microsoft Teams görünür

Kuruluş şemasında bir veya birden çok kişi devre dışı bırakılmış veya kaldırılmışsa ve profil fotoğrafı yine kuruluş şemasında **görünüyorsa, ShowInAddressLists** ayarının False olarak ayarlanmış olabilir: 

1. Etkin [Microsoft 365 yönetim merkezi >'ne](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) gidin ve fotoğrafın göründüğü kullanıcıları seçin. 
1. Posta sekmesini **seçin** ve Genel adres listesinde **göster seçeneğinin Hayır olarak** ayarlanmış olduğundan emin **olun.**

**ShowInAddressLists ayarını** **Hayır** olarak yapmak işe yaramadı ise, şunları kontrol edin: 

- Kullanıcı, listede alıcı listesinden Exchange. Daha fazla bilgi için [bkz. Exchange Online'da adres listelerini yönetme.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- Kullanıcı, posta listesinde adres listesinden Azure Active Directory. Daha fazla bilgi için bkz. [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 