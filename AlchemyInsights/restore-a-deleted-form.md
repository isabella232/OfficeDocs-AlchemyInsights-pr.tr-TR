---
title: Silinmiş formu geri yükleme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2547"
- "9000672"
ms.openlocfilehash: 6923c15c3cce90c98ae79181e978fba273ab6059
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662453"
---
# <a name="restore-a-deleted-form"></a><span data-ttu-id="8730f-102">Silinmiş formu geri yükleme</span><span class="sxs-lookup"><span data-stu-id="8730f-102">Restore a deleted form</span></span>

<span data-ttu-id="8730f-103">Microsoft Forms 'ta formu yanlışlıkla sildiyseniz, kurtarabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8730f-103">If you deleted a form in Microsoft Forms by accident, you can recover it.</span></span> <span data-ttu-id="8730f-104">Silinen formun sahibi olarak Microsoft Forms 'ta oturum açın.</span><span class="sxs-lookup"><span data-stu-id="8730f-104">Sign in to Microsoft Forms as the owner of the deleted form.</span></span> <span data-ttu-id="8730f-105">**Geri dönüşüm**kutusu 'nu seçip kurtarmak istediğiniz formu seçip **geri yükle**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="8730f-105">Select the **Recycle Bin**, then select the form you want to recover and select **Restore**.</span></span> <span data-ttu-id="8730f-106">Yüklendikten sonra, **formlarıma dön sayfa** okunun</span><span class="sxs-lookup"><span data-stu-id="8730f-106">Once restored, select the **Back to my Forms page** arrow.</span></span>

<span data-ttu-id="8730f-107">Yalnızca formun sahibi kurtarabilir.</span><span class="sxs-lookup"><span data-stu-id="8730f-107">Only the owner of the form can recover it.</span></span> <span data-ttu-id="8730f-108">Form sahibinin hesabı kiracıdan devre dışı bırakılmışsa veya kaldırıldıysa, yalnızca genel yönetici formu kurtarabilir.</span><span class="sxs-lookup"><span data-stu-id="8730f-108">If form owner's account was disabled or removed from the tenant, only the Global Administrator can recover the form.</span></span> <span data-ttu-id="8730f-109">Genel yöneticinin geri yükleme gerçekleştirmek için bir Forms Lisansı olmalıdır.</span><span class="sxs-lookup"><span data-stu-id="8730f-109">The Global Administrator must have a Forms license to perform a restore.</span></span> <span data-ttu-id="8730f-110">Yalnızca Kullanıcı hesabının, kiracı 'dan devre dışı bırakılmakta olan 30 gün içinde oluşturulan formlar geri yüklenebilir.</span><span class="sxs-lookup"><span data-stu-id="8730f-110">Only forms created within 30 days of the user account being disabled or removed from the tenant can be restored.</span></span>

<span data-ttu-id="8730f-111">Kiracının genel yöneticisiyseniz ve silinen veya devre dışı bırakılmış bir hesaptan bir formu kurtarmak istiyorsanız, şu URL 'de silinen veya devre dışı bırakılmış kullanıcının e-posta adresi [e-posta adresi] yerine bu URL 'yi koyun: \*\* https://forms.office.com/Pages/delegatepage.aspx?originalowner= [e-posta adresi]\*\* Örneğin, e-posta ADRESINIZ johndoe@contoso.com ise URL şöyle **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com** olur:</span><span class="sxs-lookup"><span data-stu-id="8730f-111">If you are the Global Administrator of the tenant, and you want to recover a form from an account that was deleted or disabled, replace [email address] with the email address of the deleted or disabled user in the following URL: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=[email address]** For example, if your email address is johndoe@contoso.com, the URL would be: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com**.</span></span> 

<span data-ttu-id="8730f-112">Kullanıcının silinen formlara erişim edindikten sonra, taşımak istediğiniz formu seçin ve ardından **diğer form eylemleri**  >  **Taşı**'yı seçin.</span><span class="sxs-lookup"><span data-stu-id="8730f-112">Once you have access to the user's deleted forms, select the form you want to move, and then select **More Form Actions** > **Move**.</span></span>

<span data-ttu-id="8730f-113">Silindiği ve kullanıcının kuruluştan kaldırıldığı bir formu kurtarmak istiyorsanız, genel yönetici kullanıcıyı kurtarmayı seçebilir, söz konusu kullanıcının parolasını sıfırlayabilir ve bu kullanıcı olarak oturum açarak forma erişerek başka bir etkin kullanıcıya taşıyabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="8730f-113">If you want to recover a form where it was deleted and the user was removed from the organization, a Global Administrator can choose to recover the user, reset the password for that user, and then while logged in as that user, access the form to move it to another active user.</span></span> 