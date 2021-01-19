---
title: Problemas con la instalación de Microsoft Defender en Mac o Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768465"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problemas con la instalación de Microsoft Defender en Mac o Linux

**Mac**

- Asegúrese de que se cumplen los requisitos de sistema antes de instalar ATP de Microsoft Defender para Mac. Para más información, consulte [Cómo instalar ATP de Microsoft Defender para Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Revise la información del archivo: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Asegúrese de que se cumplen los requisitos de sistema antes de instalar ATP de Microsoft Defender para Linux. Para más información, consulte [Cómo instalar ATP de Microsoft Defender para Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Para comprobar que el servicio MDATP se está ejecutando, consulte [Error en la instalación](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    Para resolver problemas si el servicio no se está ejecutando, consulte [Pasos para resolver problemas si el servicio MDATP no se está ejecutando](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- Para consultar los pasos para comprobar la configuración del cliente, que verifica el estado del producto, y para realizar un test de detección en el archivo de texto EICAR, vea [Configuración del cliente](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Nota** Para consultar una lista de sistemas de archivo admitidos para actividad de acceso, consulte [ATP de Microsoft Defender para Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).