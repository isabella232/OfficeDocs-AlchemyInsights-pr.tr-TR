---
title: Paylaşılan posta kutusu oluşturulurken proxy adresi hatası
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568310"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="b72ec-102">Posta kutusu veya e-posta etkinleştirilmiş başka bir nesne oluşturulurken proxy adresi hatası</span><span class="sxs-lookup"><span data-stu-id="b72ec-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="b72ec-103">E-posta özelliği etkin bir nesne (posta kutusu, paylaşılan posta kutusu vb.) oluşturmayı denediy ve ""SMTP:alias@domain.com" ara sunucu adresi zaten kullanılıyor..." hatasını alırsanız, seçtiğiniz e-posta adresi zaten kuruluşta başka bir e-posta özelliği etkin nesne tarafından kullanılıyordur.</span><span class="sxs-lookup"><span data-stu-id="b72ec-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="b72ec-104">Bu e-posta adresini içeren kullanıcı, grup, paylaşılan posta kutusu veya ortak klasörü bulmalı ve silmeli veya e-posta adresini değiştirsin.</span><span class="sxs-lookup"><span data-stu-id="b72ec-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="b72ec-105">Ardından, serbest e-posta adresine sahip yeni bir e-posta özelliği etkin nesne oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="b72ec-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="b72ec-106">Bulmak için Giriş sayfasında Ara'ya tıklayın.</span><span class="sxs-lookup"><span data-stu-id="b72ec-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="b72ec-107">Ayrıca, aramak için aşağıdaki Exchange Online PowerShell komutunu da kullanabilirsiniz:</span><span class="sxs-lookup"><span data-stu-id="b72ec-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="b72ec-108">Var olan e-posta adresini silmek istemiyorsanız, oluşturmakta olduğu yeni nesne için yeni bir e-posta adresi seçin.</span><span class="sxs-lookup"><span data-stu-id="b72ec-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  