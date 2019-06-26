---
title: SharePoint veya OneDrive erişimi sınırlama
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223732"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>SharePoint veya OneDrive erişimi sınırlama

SharePoint çevrimiçi/OneDrive hizmetlerine erişimi kısıtlamak için birçok yol vardır. Bu çeşitli erişim kısıtlama yöntemleri aşağıda özetlenmiştir. 

**İzni kısıtlama**

SharePoint çevrimiçi ve iş OneDrive, biz siteleri, dosyalar ve klasörler gibi öğeleri erişimi olmalıdır bu gruplar/kişiler erişim vererek kısıtlayın.

- [SharePoint liste veya kitaplık izinlerini Özelleştir](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint site izinlerini özelleştirme](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Bir alt klasör izinlerini değiştirme](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Yönetilmeyen cihazlardan erişimi denetleme](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePoint veya Office 365'te genel yönetim bloke edebilir veya yönetilmeyen aygıtlardan SharePoint ve OneDrive içeriğe erişimi sınırlama (Bu karma AD birleştirilmiş veya Intune uyumlu).

**Ağ konumu kısıtlama**

Bir BT yöneticisi, güvendiğiniz tanımlanan ağ konumlarına dayalı SharePoint ve OneDrive kaynaklarına erişimi denetleyebilirsiniz. Konum temelli ilke olarak da budur. Daha fazla bilgi için lütfen [SharePoint çevrimiçi ve ağ konumuna bağlı olarak OneDrive veri erişimi denetleme](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) bkz:

**Site kilit kısıtlaması** 

SharePoint içinde çevrimiçi erişimi olan hiç kimse için bir site koleksiyonu kilitleme olanağı vardır. Bu PowerShell ve [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState özelliğini kullanarak [SharePoint çevrimiçi Yönetimi Kabuk](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) aracılığıyla ayarlanır.

**Kullanıcıların site veya alt site oluşturmasını kısıtlamak**

SharePoint Yönetim veya Office 365 genel yönetici, kullanıcılarınızın oluşturmak ve kendi SharePoint sitelerini yönetmek, bunlar ne tür siteler oluşturabilir, belirlemek sağlayabilirsiniz ve siteleri konumunu belirtin. Daha fazla bilgi için lütfen bkz [Yönet Online'da SharePoint sitesi oluşturma](https://docs.microsoft.com/sharepoint/manage-site-creation)

