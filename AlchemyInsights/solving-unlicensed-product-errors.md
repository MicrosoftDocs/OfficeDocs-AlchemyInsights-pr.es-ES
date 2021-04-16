---
title: Solución de errores de producto sin licencia
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
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786866"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Sugerencias para resolver errores de "Producto sin licencia"

Para solucionar errores sobre un "Producto sin licencia", pruebe lo siguiente:

- Comprueba si el estado de la suscripción ha expirado.
- Asegúrese de que tiene una suscripción que permite licencias de cliente, como Aplicaciones de Microsoft 365 para empresas o Empresa Premium, y asegúrese de que el usuario tiene asignada una [licencia](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Asegúrese de que el usuario inicia sesión en Office con la misma cuenta que tiene asignada la licencia.
- Compruebe la [página Estado del servicio](https://docs.microsoft.com/office365/enterprise/view-service-health) para ver si hay algún problema conocido con el servicio.
- Comprueba la configuración del firewall, el software antivirus y el proxy para confirmar que no bloquean el acceso de aplicaciones de Microsoft 365 a Internet. Consulte [DIRECCIONES URL e intervalos de direcciones IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

También puede probar las siguientes acciones de solución de problemas: 

- Abra una aplicación de Office y [salga de](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) cualquier cuenta de usuario existente. [Quite](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) y [vuelva a asignar la](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licencia de Office y, a continuación, inicie sesión en [Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) con la cuenta de usuario afectada.
- Ejecute el [solucionador de problemas de activación](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Restablezca el estado de activación de Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Realizar una reparación en línea de Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Para ver más medidas de solución de problemas, vea: 

- [Errores de activación y de producto sin licencia en Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Error "Lo sentimos, no podemos conectarnos con su cuenta. Inténtelo de nuevo más tarde" al activar Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)