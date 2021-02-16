---
title: Cihaz Geri Yazma
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
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256972"
---
# <a name="device-writeback"></a><span data-ttu-id="36090-102">Cihaz Geri Yazma</span><span class="sxs-lookup"><span data-stu-id="36090-102">Device Writeback</span></span>

<span data-ttu-id="36090-103">Cihaz Geri Yazma aşağıdaki senaryolarda kullanılır:</span><span class="sxs-lookup"><span data-stu-id="36090-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="36090-104">Karma [sertifika güveni dağıtımını kullanarak İş için Windows Hello'ya etkinleştirme](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="36090-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="36090-105">AdFS (2012 R2 veya daha yüksek) korumalı uygulamalara (bağlı olan taraf güvenlerine bağlı) cihazlara dayalı olarak Koşullu Erişimi etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="36090-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="36090-106">Cihaz geri yazma için Azure AD Premium aboneliği gereklidir.</span><span class="sxs-lookup"><span data-stu-id="36090-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="36090-107">Bu, uygulamalara erişimin yalnızca güvenilen cihazlara verilmesini sağlayan ek güvenlik ve güvence sağlar.</span><span class="sxs-lookup"><span data-stu-id="36090-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="36090-108">Koşullu Erişim hakkında daha fazla bilgi için bkz. Koşullu Erişimle [Riski](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) Yönetme ve Azure Active Directory Cihaz Kaydı'ı kullanarak Şirket İçi Koşullu Erişimi [Ayarlama.](https://docs.microsoft.com/azure/active-directory/devices/overview)</span><span class="sxs-lookup"><span data-stu-id="36090-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="36090-109">Cihazlar için Cihaz Geri Yazma özelliğini etkinleştirme hakkında daha fazla bilgi için bkz. Cihaz Geri [Yazma özelliğini etkinleştirme.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)</span><span class="sxs-lookup"><span data-stu-id="36090-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
