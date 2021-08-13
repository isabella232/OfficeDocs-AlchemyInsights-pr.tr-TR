---
title: E-posta veya SharePoint erişimi OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093909"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>E-posta veya SharePoint erişimi OneDrive

SharePoint Online/OneDrive hizmetleri için erişimi kısıtlamanın birçok yolu vardır. Bu çeşitli erişim kısıtlama yöntemleri aşağıda açıklanmıştır. 

**İzin Kısıtlaması**

SharePoint Online ve OneDrive İş'da, yalnızca erişime sahip olması gereken gruplara/kişilere erişim izni vererek siteler, dosyalar ve klasörler gibi öğelere erişimi kısıtlarız.

- [Liste veya kitaplığın SharePoint özelleştirme](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Site SharePoint özelleştirme](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alt klasör izinlerini değiştirme](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Yönetilmeyen cihazlardan erişimi denetleme](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Bir SharePoint yöneticisi veya genel yönetici olarak, yönetnemeyen cihazlardan (Intune'da karma AD'ye katılan veya uyumlu olmayanlar) SharePoint ve OneDrive içeriğine erişimi engelleyebilir veya sınırlandırabilirsiniz.

**Ağ Konumu Kısıtlaması**

Bir IT yöneticisi olarak, güvenilen tanımlı ağ konumlarına SharePoint OneDrive kaynak erişimi ve kaynak OneDrive denetlemeniz gerekir. Bu, konum tabanlı ilke olarak da bilinir. Daha fazla bilgi için lütfen SharePoint [Online'a](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) erişimi denetleme ve OneDrive konuma göre verileri denetleme

**Site Kilidi Kısıtlaması** 

SharePoint Online'da, site koleksiyonunu kilitleme olanağına sahip olur, böylece kimse erişimini kilitler. Bu, [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState [özelliği kullanılarak](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) PowerShell SharePoint Çevrimiçi Yönetim Kabuğu ile ayarlanır.

**Kullanıcıların site veya alt site oluşturmasını kısıtlama**

Genel SharePoint veya Genel yönetici olarak, kullanıcılarınızı kendi SharePoint sitelerini oluşturmalarına ve yönetmelerine, ne tür siteler oluştur oluşturduklarını belirlemelerine ve sitelerin konumunu belirtmelerine izin veebilirsiniz. Daha fazla bilgi için bkz. [SharePoint Online'da site SharePoint yönetme](https://docs.microsoft.com/sharepoint/manage-site-creation)

