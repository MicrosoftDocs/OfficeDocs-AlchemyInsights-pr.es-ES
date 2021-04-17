---
title: Iniciar sesión en Windows 10 sin usar una contraseña
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830563"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Iniciar sesión en Windows 10 sin usar una contraseña

Para evitar tener que escribir una contraseña en el inicio de Windows, te recomendamos que uses una de las opciones de inicio de sesión seguro de Windows Hello, como un PIN, reconocimiento facial o huella digital, si está disponible. Si realmente quieres deshabilitar el inicio de sesión seguro, consulta las instrucciones "Iniciar sesión automáticamente en Windows 10" a continuación.

**Alternativas seguras de Windows Hello a la contraseña de la cuenta**

Ve a **Configuración > cuentas > opciones de inicio** de sesión (o haz clic [aquí).](ms-settings:signinoptions?activationSource=GetHelp) Aparecerán las opciones de inicio de sesión disponibles. Por ejemplo:

![Opciones de inicio de sesión.](media/sign-in-options.png)

Haga clic o pulse en una de las opciones para configurarla. La próxima vez que inicies o desbloquees Windows, podrás usar la nueva opción en lugar de una contraseña. 

**Iniciar sesión automáticamente en Windows 10**

**Nota:** El inicio de sesión automático es conveniente, pero presenta un riesgo de seguridad, especialmente si el equipo es accesible por varias personas. 

1. Haga clic o pulse en **el botón** Inicio de la barra de tareas.

2. Escriba **netplwiz** y presione la tecla Entrar para abrir la ventana Cuentas de usuario.

3. En **Cuentas de usuario,** haz clic en la cuenta en la que quieres iniciar sesión automáticamente cuando se inicie Windows.

4. Desactive la casilla "Los usuarios deben escribir un nombre de usuario y una contraseña para usar este equipo".

    ![Los usuarios deben escribir una opción de nombre de usuario y contraseña.](media/users-must-enter-username.png)

5. Haga clic en **Aceptar**. Se le pedirá que escriba y confirme la contraseña de la cuenta que seleccionó. Haga clic en **Aceptar** para finalizar. La próxima vez que se inicie Windows 10, iniciará sesión automáticamente en la cuenta seleccionada.
