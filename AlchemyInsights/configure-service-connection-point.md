---
title: Hizmet Bağlantı Noktasını (SCP) Yapılandırma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037292"
---
# <a name="configure-service-connection-point-scp"></a>Hizmet bağlantı noktasını (SCP) yapılandırma

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Neden:** SCP nesnesi okunamıyor ve Azure AD kiracı bilgilerine ulaşamıyor
- **Çözüm:** Hizmet Bağlantı Noktası [Yapılandırma bölümüne bakın](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Eylem planı**

- Cihazın denetimli doğrulama için GPO'ya sahip olup olmadığını kontrol edin.
- GPO'nun kayıt defteri anahtarlarını oluşturduğuna emin olun.
- Dizin kimliği ve onmicrosoft etki alanıyla 2 anahtar oluşturduğunuzdan emin olun.

**SCP için istemci tarafı kayıt defteri ayarını yapılandırma**

Cihazlarınızı kayıt defterinde SCP girdisini yapılandıran bir kayıt defteri ayarını dağıtmak üzere Grup İlkesi Nesnesi (GPO) oluşturmak için aşağıdaki örneği kullanın.

1. Grup İlkesi Yönetim konsolu açın ve etki alanınıza yeni bir GPO oluşturun.
     - Yeni oluşturduğunuz GPO'ya bir ad verin (örneğin, ClientSideSCP)

2. GPO'u düzenleyin ve şu yolu bulun: Bilgisayar **Yapılandırması > Tercihleri ve Windows > Ayarları > Defteri.**

3. Kayıt Defteri'ne **sağ tıklayın** ve Kayıt **Defteri >'ni seçin.**

4. Genel **sekmesinde,** aşağıdakini yapılandırabilirsiniz:
  
- **Eylem**: Güncelleştirme
    
- **Kurye**: HKEY_LOCAL_MACHINE
    
- **Anahtar Yolu:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Değer adı**: TenantId
    
- **Değer türü:** REG_SZ
    
- **Değer verileri:** Azure AD örneğinizin GUID veya Dizin Kimliği (Bu değer Azure portalında > **Azure Active Directory > Özellikleri > Dizin Kimliği)**
 
- **Tamam**'a tıklayın.
 
5. Kayıt Defteri'ne **sağ tıklayın** ve Kayıt **Defteri >'ni seçin.**

6. Genel **sekmesinde,** aşağıdakini yapılandırabilirsiniz:
  
- **Eylem**: Güncelleştirme
    
- **Kurye**: HKEY_LOCAL_MACHINE
    
- **Anahtar Yolu:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Değer adı**: TenantName
    
- **Değer türü:** REG_SZ
    
- **Değer verileri:** AD FS gibi bir federasyon ortamı kullanıyorsanız, doğrulanmış etki alanı adınız. Yönetilen bir ortam kullanıyorsanız, onmicrosoft.com etki alanı adınız (örneğin, contoso.onmicrosoft).com

- **Tamam**'a tıklayın.

7. Yeni oluşturulan GPO için düzenleyiciyi kapatın.

8. Yeni oluşturulan GPO'nun bağlantısını, denetimli olarak açılan popülasyona ait etki alanına katılmış bilgisayarları içeren istenen OU'ya bın.

Daha fazla bilgi için bkz. Karma Azure AD birleştirme [denetimli doğrulaması - Azure AD | Microsoft Belgeler ve Sorun](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)  [Giderme karma Azure Active Directory'ye katılmış cihazlar ve | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









