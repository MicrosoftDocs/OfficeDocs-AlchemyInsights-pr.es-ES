---
title: 1048 5.7.750 servicio no disponible. El cliente bloqueó el envío de dominios no registrados
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom: 1048
ms.openlocfilehash: 5eb42679f123fcd1b680327329721cb47e18e11a
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776518"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a>el cliente de 5.7.750 bloqueó el envío desde un dominio no registrado

El error se produce cuando se envía un gran volumen de mensajes desde dominios que no se aprovisionan en Office 365 (que se agregan como dominios aceptados y se validan).
  
Para evitar este error, puede usar un conector de flujo de correo basado en certificados donde el dominio del certificado sea un dominio aprovisionado o puede aprovisionar todos los dominios de envío.
  
