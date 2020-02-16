---
title: Office Uygulamalarını Düzeltme Hesabınız kötü bir durum iletisi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969891"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="ca779-102">Office uygulamalarını düzeltme "Hesabınız kötü durumda" hatası</span><span class="sxs-lookup"><span data-stu-id="ca779-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="ca779-103">Bu hatayı düzeltmek için etkilenen bilgisayarda aşağıdaki seçenekleri deneyin:</span><span class="sxs-lookup"><span data-stu-id="ca779-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="ca779-104">Bir Office uygulaması açın, tüm hesaplardan **Dosya** > **Hesabı** > **Oturum Aç'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="ca779-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="ca779-105">Geçerli bir lisansa sahip bir kullanıcı hesabı kullanarak yeniden oturum açın.</span><span class="sxs-lookup"><span data-stu-id="ca779-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="ca779-106">Ayrıntılı bilgi için [Bkz. Ofis'teki Hesaplar.](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)</span><span class="sxs-lookup"><span data-stu-id="ca779-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="ca779-107">Windows Kimlik Bilgileri Yöneticisi'ni kullanarak [Office kimlik bilgilerini temizleyin.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)</span><span class="sxs-lookup"><span data-stu-id="ca779-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="ca779-108">**Not:** Office 2016'nın kayıt defteri yolları 16.0 olarak değiştirildi.</span><span class="sxs-lookup"><span data-stu-id="ca779-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="ca779-109">Örneğin, \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="ca779-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="ca779-110">Etkilenen bilgisayarda Aşağıdaki adımları kullanarak EnableADAL = 0'ı ayarlayın:</span><span class="sxs-lookup"><span data-stu-id="ca779-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="ca779-111">Windows düğmesine sağ tıklayın ve **Çalıştır'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="ca779-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="ca779-112">**Açık** kutusunda **regedit**yazın ve ardından **Tamam'ı**seçin.</span><span class="sxs-lookup"><span data-stu-id="ca779-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="ca779-113">Kayıt Defteri Düzenleyicisi'nin cihazınızda değişiklik yapmasına izin vermek istendiğinde **Evet'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="ca779-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="ca779-114">Kayıt Defteri Düzenleyicisi'nde, HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity altında 0 ayarı olan EnableADAL'ın DWORD değerini ekleyin.</span><span class="sxs-lookup"><span data-stu-id="ca779-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="ca779-115">Office 2013'u kullanarak Office 365'e bağlanırken hata oluşursa, Office [istemcisi için modern kimlik doğrulamasını etkinleştirin.](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)</span><span class="sxs-lookup"><span data-stu-id="ca779-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="ca779-116">Daha fazla bilgi için, [Office 365, Azure veya Intune'da oturum açamayan tarayıcı dışı uygulamaların nasıl giderilene](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)bakınız.</span><span class="sxs-lookup"><span data-stu-id="ca779-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

