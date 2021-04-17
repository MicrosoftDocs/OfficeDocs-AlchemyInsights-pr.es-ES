---
title: Facturación moderna de correo electrónico de Azure
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
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820843"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="2a338-102">Facturación de correo electrónico en Azure</span><span class="sxs-lookup"><span data-stu-id="2a338-102">Email invoicing in Azure</span></span>

<span data-ttu-id="2a338-103">Debes tener un rol de propietario o colaborador en el perfil de facturación o en su cuenta de facturación para actualizar su preferencia de facturación por correo electrónico.</span><span class="sxs-lookup"><span data-stu-id="2a338-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="2a338-104">Una vez que haya optado por recibir, todos los usuarios con funciones de propietario, colaborador, lector y gestor de facturas en un perfil de facturación recibirán su factura por correo electrónico.</span><span class="sxs-lookup"><span data-stu-id="2a338-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="2a338-105">Inicie sesión en el [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="2a338-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="2a338-106">Buscar la **administración de costos + facturación**.</span><span class="sxs-lookup"><span data-stu-id="2a338-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="2a338-107">Seleccione **Facturas** en la parte izquierda y, a continuación, seleccione **Factura de correo electrónico** desde la parte superior de la página.</span><span class="sxs-lookup"><span data-stu-id="2a338-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="2a338-108">Si tiene varios perfiles de facturación, seleccione un perfil de facturación y, a continuación, seleccione **optar por recibir**.</span><span class="sxs-lookup"><span data-stu-id="2a338-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="2a338-109">Seleccione **Actualizar**.</span><span class="sxs-lookup"><span data-stu-id="2a338-109">Select **Update**.</span></span>
6. <span data-ttu-id="2a338-110">Si tiene varios perfiles de facturación, seleccione un perfil de facturación y, a continuación, seleccione **optar por recibir**.</span><span class="sxs-lookup"><span data-stu-id="2a338-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="2a338-111">Para conceder acceso a otros usuarios para ver, descargar y pagar facturas, debe asignarles el rol de administrador de facturas para un perfil de facturación MCA o MPA.</span><span class="sxs-lookup"><span data-stu-id="2a338-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="2a338-112">Si ha optado por recibir su factura en el correo electrónico, los usuarios también recibirán las facturas por correo electrónico.</span><span class="sxs-lookup"><span data-stu-id="2a338-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="2a338-113">Inicie sesión en el [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="2a338-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="2a338-114">Buscar la **administración de costos + facturación**.</span><span class="sxs-lookup"><span data-stu-id="2a338-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="2a338-115">Seleccione **Perfiles de facturación** en la parte izquierda.</span><span class="sxs-lookup"><span data-stu-id="2a338-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="2a338-116">En la lista perfiles de facturación, seleccione un perfil de facturación al que quiera asignar un rol de administrador de facturas.</span><span class="sxs-lookup"><span data-stu-id="2a338-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="2a338-117">Seleccione **Access Control (IAM)** desde el lado izquierdo y, a continuación, seleccione **Agregar** desde la parte superior de la página.</span><span class="sxs-lookup"><span data-stu-id="2a338-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="2a338-118">En la lista desplegable Rol, seleccione **administrador de facturas**.</span><span class="sxs-lookup"><span data-stu-id="2a338-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="2a338-119">Escriba la dirección de correo electrónico del usuario para dar acceso.</span><span class="sxs-lookup"><span data-stu-id="2a338-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="2a338-120">Seleccione **Guardar** para asignar el rol.</span><span class="sxs-lookup"><span data-stu-id="2a338-120">Select **Save** to assign the role.</span></span>
