---
title: ¿Necesita marcar un dominio o remitente de correo electrónico como seguro?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792149"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="4e79e-102">¿Necesita marcar un dominio o remitente de correo electrónico como seguro?</span><span class="sxs-lookup"><span data-stu-id="4e79e-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="4e79e-103">No se recomienda el uso de **listas de remitentes seguros** ya que expone su organización a ataques de spam, phishing y suplantación de identidad.</span><span class="sxs-lookup"><span data-stu-id="4e79e-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="4e79e-104">Sin embargo, si hay un requisito empresarial, **recomendamos** usar **[Reglas de flujo de correo](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** para esto.</span><span class="sxs-lookup"><span data-stu-id="4e79e-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="4e79e-105">Nuestra guía garantiza la autenticación del remitente (comprueba que el dominio remitente no está falsificado).</span><span class="sxs-lookup"><span data-stu-id="4e79e-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="4e79e-106">**Nota**: no recomendamos administrar los falsos positivos con las listas de remitentes seguros, ya que las excepciones al filtrado de correo no deseado pueden exponer la organización a ataques de seguridad.</span><span class="sxs-lookup"><span data-stu-id="4e79e-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="4e79e-107">Si los usuarios reciben mensajes que se marcan incorrectamente como spam o correo electrónico no deseado, puede **[Informar de los mensajes y archivos a Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="4e79e-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="4e79e-108">**Deberían evitarse** los remitentes seguros en Outlook, la lista de remitentes permitidos o la lista de dominios permitidos en las directivas antispam porque los remitentes omiten toda la protección contra correo no deseado, suplantación de identidad, protección contra phishing y autenticación de remitente (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="4e79e-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="4e79e-109">Este método es más adecuado solo para las pruebas temporales.</span><span class="sxs-lookup"><span data-stu-id="4e79e-109">This method is best used for temporary testing only.</span></span>
