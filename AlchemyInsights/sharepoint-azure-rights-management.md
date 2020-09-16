---
title: SharePoint veya OneDrive 'da erişimi kısıtlama
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: cc6f93ba8ae3a030f83da5eca2d28dcf38f0f8f7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47800916"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="4b226-102">SharePoint dosyalarına ıRM koruması</span><span class="sxs-lookup"><span data-stu-id="4b226-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="4b226-103">SharePoint Online 'da, liste ve kitaplık düzeyindeki dosyalara ıRM koruması uygulanır.</span><span class="sxs-lookup"><span data-stu-id="4b226-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="4b226-104">Kuruluşunuzun ıRM korumasını kullanabilmesi için önce hak yönetimini ayarlamanız gerekir.</span><span class="sxs-lookup"><span data-stu-id="4b226-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="4b226-105">IRM, kullanım kısıtlamalarını şifrelemek ve atamak için Azure Information Protection 'dan Azure Rights Management hizmetine bağımlıdır.</span><span class="sxs-lookup"><span data-stu-id="4b226-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="4b226-106">Bazı Microsoft 365 abonelikleri Azure Rights Management 'ı içerir, ancak tümünü desteklemez.</span><span class="sxs-lookup"><span data-stu-id="4b226-106">Some Microsoft 365 subscriptions include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="4b226-107">Daha fazla bilgi için şu makalelere bakın:</span><span class="sxs-lookup"><span data-stu-id="4b226-107">To learn more, see:</span></span>

- <span data-ttu-id="4b226-108">[Office uygulamaları ve Hizmetleri Azure Rights Management 'ı nasıl destekler](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span><span class="sxs-lookup"><span data-stu-id="4b226-108">[How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="4b226-109">[SharePoint Yönetim merkezinde bilgi hakları yönetimi 'ni (IRM) ayarlayın](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center).</span><span class="sxs-lookup"><span data-stu-id="4b226-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center).</span></span>

- <span data-ttu-id="4b226-110">[IRM-SharePoint belge kitaplıklarını ve listelerini etkinleştirin](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span><span class="sxs-lookup"><span data-stu-id="4b226-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="4b226-111">[Office 'Te bilgi hakları yönetimi](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span><span class="sxs-lookup"><span data-stu-id="4b226-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span></span>

- <span data-ttu-id="4b226-112">[Exchange Online 'Da bilgi hakları yönetimi](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="4b226-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online).</span></span>


