---
title: Administrar la lista global de direcciones y la libreta de direcciones sin conexión de la organización
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
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794849"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="8ca01-102">Administrar la lista global de direcciones (GAL) y la libreta de direcciones sin conexión (OAB) de la organización.</span><span class="sxs-lookup"><span data-stu-id="8ca01-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="8ca01-103">Una lista global de direcciones (GAL) es una lista de objetos habilitados para correo (cualquier tipo de destinatario que puede recibir un correo electrónico) en la organización.</span><span class="sxs-lookup"><span data-stu-id="8ca01-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="8ca01-104">Se crea automáticamente una GAL en cada organización.</span><span class="sxs-lookup"><span data-stu-id="8ca01-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="8ca01-105">Puede crear GAL adicionales para separar usuarios por organización o ubicación, pero un único usuario solo puede ver y usar una GAL cada vez.</span><span class="sxs-lookup"><span data-stu-id="8ca01-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="8ca01-106">Algunos clientes de correo electrónico, como Outlook para Windows, descargan la GAL para su uso sin conexión.</span><span class="sxs-lookup"><span data-stu-id="8ca01-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="8ca01-107">Esto se conoce como libreta de direcciones sin conexión (OAB).</span><span class="sxs-lookup"><span data-stu-id="8ca01-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="8ca01-108">En Exchange Online, una OAB se actualiza solo cada 8 horas. A continuación, los clientes deben descargarla para actualizar la copia de OAB local.</span><span class="sxs-lookup"><span data-stu-id="8ca01-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="8ca01-109">Los cambios en los destinatarios deben ser visibles en primer lugar en la GAL para convertirlos más tarde en la OAB.</span><span class="sxs-lookup"><span data-stu-id="8ca01-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="8ca01-110">Estos son algunos de los procedimientos más utilizados para GAL y OAB:</span><span class="sxs-lookup"><span data-stu-id="8ca01-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="8ca01-111">Por varios motivos, es posible que desee ocultar algunos objetos de la GAL.</span><span class="sxs-lookup"><span data-stu-id="8ca01-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="8ca01-112">Vea [Ocultar destinatarios de las listas de direcciones](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="8ca01-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="8ca01-113">Si necesita dar a grupos específicos de usuarios vistas personalizadas de la GAL de la organización, consulte [Directivas de libreta de direcciones en Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="8ca01-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="8ca01-114">[Cree una lista de direcciones global en Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) y para obtener información sobre cómo trabajar con los permisos de GAL, vea [Listas de direcciones de Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="8ca01-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="8ca01-115">Tenga en cuenta que, si crea nuevas GAL, es posible que también quiera crear una nueva OAB.</span><span class="sxs-lookup"><span data-stu-id="8ca01-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="8ca01-116">Consulte [Procedimientos de libretas de direcciones sin conexión](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="8ca01-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
