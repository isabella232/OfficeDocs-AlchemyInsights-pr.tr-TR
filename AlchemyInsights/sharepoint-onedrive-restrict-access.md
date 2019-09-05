---
title: SharePoint veya OneDrive'da erişimi kısıtlama
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750684"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>SharePoint veya OneDrive'da erişimi kısıtlama

SharePoint Online/OneDrive hizmetlerine erişimi kısıtlamanın birçok yolu vardır. Bu çeşitli erişim kısıtlama yöntemleri aşağıda özetlenmiştir. 

**İzin Kısıtlaması**

SharePoint Online ve OneDrive for Business'ta, siteler, dosyalar ve klasörler gibi öğelere erişimi yalnızca erişimi olması gereken gruplara/kişilere erişim izni vererek kısıtlarız.

- [SharePoint listesi veya kitaplık için izinleri özelleştirme](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint site izinlerini özelleştirme](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alt klasördeki izinleri değiştirme](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Yönetilmeyen cihazlardan erişimi denetleme](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Office 365'te SharePoint veya global yönetici olarak, yönetilmeyen aygıtlardan SharePoint ve OneDrive içeriğine erişimi engelleyebilir veya sınırlandırabilirsiniz (Karma AD'nin Intune'da katıldığı veya uyumlu olmayanlar).

**Ağ Konumu Kısıtlaması**

BT yöneticisi olarak, güvendiğiniz tanımlı ağ konumlarını temel alan SharePoint ve OneDrive kaynaklarına erişimi denetleyebilirsiniz. Bu, konum tabanlı ilke olarak da bilinir. Daha fazla bilgi için lütfen [ağ konumuna göre SharePoint Online ve OneDrive verilerine erişimi kontrol etme](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) konusuna bakın

**Site Kilidi Kısıtlaması** 

SharePoint Online'da bir site koleksiyonunu kilitleme olanağınız vardır, böylece kimsenin erişimi yoktur. Bu [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState özelliği kullanılarak PowerShell ve [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) üzerinden ayarlanır.

**Kullanıcıların site veya alt site oluşturmalarını kısıtlama**

SharePoint yöneticisi veya Office 365 global yöneticisi olarak, kullanıcılarınızın kendi SharePoint sitelerini oluşturmasına ve yönetmesine, ne tür siteler oluşturabileceklerini belirlemesine ve sitelerin konumunu belirtebildiği ne kadar sınamasına izin verebilirsiniz. Daha fazla bilgi için lütfen [SharePoint Online'da site oluşturmayı yönet'e](https://docs.microsoft.com/sharepoint/manage-site-creation) bakın

