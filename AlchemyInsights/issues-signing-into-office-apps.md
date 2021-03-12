---
title: Problemas al iniciar sesión en aplicaciones de Microsoft 365
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
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709123"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="a4d0a-102">Corregir las aplicaciones de Microsoft 365 Mensaje "El módulo de plataforma de confianza del equipo no funciona correctamente"</span><span class="sxs-lookup"><span data-stu-id="a4d0a-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="a4d0a-103">Para corregir este error, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="a4d0a-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="a4d0a-104">Instalar las actualizaciones más recientes [para Windows](https://support.microsoft.com/help/4027667/windows-10-update) y [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="a4d0a-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="a4d0a-105">[Borra las credenciales de Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) con el Administrador de credenciales de Windows.</span><span class="sxs-lookup"><span data-stu-id="a4d0a-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="a4d0a-106">**Nota:** Las rutas de acceso del Registro para Office 2016 han cambiado a 16.0.</span><span class="sxs-lookup"><span data-stu-id="a4d0a-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="a4d0a-107">(Por ejemplo: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="a4d0a-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="a4d0a-108">Pruebe el [proceso de recuperación del usuario](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) para corregir errores del Módulo de plataforma segura (TPM).</span><span class="sxs-lookup"><span data-stu-id="a4d0a-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="a4d0a-109">Establezca EnableADAL = 0 siguiendo los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="a4d0a-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="a4d0a-110">Haga clic con el botón secundario en el botón Inicio de Windows, elija **Ejecutar**, escriba **regedit** y, a continuación, elija **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="a4d0a-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="a4d0a-111">Selecciona **Sí** para permitir que el Editor del Registro realice cambios en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a4d0a-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="a4d0a-112">En el Editor del Registro, agregue un valor DWORD de **EnableADAL** con una configuración de **0** en HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="a4d0a-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="a4d0a-113">Para obtener más información, vea [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="a4d0a-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>