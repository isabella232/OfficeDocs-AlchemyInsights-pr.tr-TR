---
title: Uygulamaları silme veya geri yükleme
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015021"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="54938-102">Uygulamaları silme veya geri yükleme</span><span class="sxs-lookup"><span data-stu-id="54938-102">Delete or restore applications</span></span>

<span data-ttu-id="54938-103">**Azure AD kiracınızdaki bir uygulamayı silmek için**:</span><span class="sxs-lookup"><span data-stu-id="54938-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="54938-104">**Azure AD portalında** **Kurumsal uygulamalar**'ı seçin.</span><span class="sxs-lookup"><span data-stu-id="54938-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="54938-105">Ardından, silmek istediğiniz uygulamayı bulun ve seçin.</span><span class="sxs-lookup"><span data-stu-id="54938-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="54938-106">Sol bölmedeki **Yönet** bölümünde **Özellikler**'i seçin.</span><span class="sxs-lookup"><span data-stu-id="54938-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="54938-107">**Sil**'i seçin ve Azure AD kiracınızdaki uygulamayı silmek istediğinizi onaylamak Için **Evet 'i** seçin.</span><span class="sxs-lookup"><span data-stu-id="54938-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="54938-108">Uygulamayı silme hakkında daha fazla bilgi için, [hızlı başlangıç: Azure Active Directory (Azure AD) kiracınızdaki bir uygulamayı silme](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="54938-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="54938-109">PowerShell 'de, [Remove-Azureadapplicationproxyapma](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet 'ı Azure Active Directory 'de belirli bir uygulamadan uygulama proxy yapılandırmalarını kaldırır ve belirtilmişse uygulamayı tamamen silebilir.</span><span class="sxs-lookup"><span data-stu-id="54938-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="54938-110">**Silinmiş bir uygulamayı PowerShell kullanarak geri yükleyebilirsiniz** .</span><span class="sxs-lookup"><span data-stu-id="54938-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="54938-111">Geri yüklemek istediğiniz uygulama tanımlandıktan sonra, [restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)kullanarak geri yükleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="54938-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
