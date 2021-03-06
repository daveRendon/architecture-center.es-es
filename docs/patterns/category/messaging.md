---
title: "Patrones de mensajería"
description: "La naturaleza distribuida de las aplicaciones en la nube requiere una infraestructura de mensajería que permite conectar los componentes y servicios, idealmente mediante un acoplamiento flexible, para maximizar la escalabilidad. La mensajería asincrónica se usa ampliamente y ofrece numerosas ventajas, pero también supone desafíos como la ordenación de los mensajes, la administración de mensajes dudosos, la idempotencia, etc."
keywords: "Patrón de diseño"
author: dragon119
ms.date: 06/23/2017
pnp.series.title: Cloud Design Patterns
ms.openlocfilehash: 6151f7f76fc7b3a953988122db75bdc25b49811f
ms.sourcegitcommit: b0482d49aab0526be386837702e7724c61232c60
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/14/2017
---
# <a name="messaging-patterns"></a>Patrones de mensajería

[!INCLUDE [header](../../_includes/header.md)]

La naturaleza distribuida de las aplicaciones en la nube requiere una infraestructura de mensajería que permite conectar los componentes y servicios, idealmente mediante un acoplamiento flexible, para maximizar la escalabilidad. La mensajería asincrónica se usa ampliamente y ofrece numerosas ventajas, pero también supone desafíos como la ordenación de los mensajes, la administración de mensajes dudosos, la idempotencia, etc.

| Patrón | Resumen |
| ------- | ------- |
| [Competing Consumers](../competing-consumers.md) | Permite que varios consumidores simultáneos procesen los mensajes recibidos en el mismo canal de mensajería. |
| [Pipes and Filters](../pipes-and-filters.md) | Desglosa una tarea que realiza un procesamiento complejo en una serie de elementos independientes que se pueden volver a utilizar. |
| [Priority Queue](../priority-queue.md) | Clasifica por orden de prioridad las solicitudes enviadas a los servicios para que aquellas con una prioridad más alta se reciban y procesen más rápidamente que las que tienen una prioridad más baja. |
| [Queue-Based Load Leveling](../queue-based-load-leveling.md) | Use una cola que actúe como búfer entre una tarea y un servicio que invoca para equilibrar cargas pesadas intermitentes. |
| [Scheduler Agent Supervisor](../scheduler-agent-supervisor.md) | Coordina un conjunto de acciones en un conjunto distribuido de servicios y otros recursos remotos. |