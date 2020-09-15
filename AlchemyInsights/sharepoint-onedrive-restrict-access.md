---
title: SharePoint veya OneDrive 'da erişimi kısıtlama
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700475"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>SharePoint veya OneDrive 'da erişimi kısıtlama

SharePoint Online/OneDrive hizmetlerine erişimi sınırlandırmanın birçok yolu vardır. Bu çeşitli erişim kısıtlama yöntemleri aşağıda özetlenmiştir. 

**İzin kısıtlaması**

SharePoint Online ve OneDrive Iş 'te, yalnızca erişmesi gereken gruplara/kişilere erişim vererek site, dosya ve klasör gibi öğelere erişimi kısıtlıyoruz.

- [SharePoint listesi veya kitaplığı için izinleri özelleştirme](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint sitesi izinlerini özelleştirme](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alt klasördeki izinleri değiştirme](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Yönetilmeyen cihazlardan erişimi denetleme](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePoint veya genel yönetici olarak, yönetilmeyen cihazlardan SharePoint ve OneDrive içeriğine erişimi engelleyebilir veya sınırlayabilir (karma AD 'a bağlı olmayan veya Intune 'da uyumlu olanlar).

**Ağ konumu kısıtlaması**

BT Yöneticisi olarak, güvendiğiniz ağ konumlarına göre SharePoint ve OneDrive kaynaklarına erişimi denetleyebilirsiniz. Bu, konum tabanlı ilke olarak da bilinir. Daha fazla bilgi için bkz: [SharePoint Online ve OneDrive verilerine ağ konumuna göre denetleme](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Site kilit sınırlaması** 

SharePoint Online 'da site koleksiyonunu kilitleme olanağınız vardır, dolayısıyla kimse erişimi yoktur. Bu, [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate özelliği kullanılarak PowerShell ve [SharePoint Online Yönetim Kabuğu](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ile ayarlanır.

**Kullanıcıların site veya alt site oluşturmasını kısıtlama**

SharePoint Yöneticisi veya genel yönetici olarak, kullanıcılarınızın kendi SharePoint sitelerini oluşturmasına ve yönetmesine, oluşturabildikleri site türlerini belirlemesine ve sitelerin konumunu belirlemesine izin verebilirsiniz. Daha fazla bilgi için bkz: [SharePoint Online 'da site oluşturmayı yönetme](https://docs.microsoft.com/sharepoint/manage-site-creation)

