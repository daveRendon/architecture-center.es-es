---
title: Patrones de resistencia
description: "La resistencia es la capacidad de un sistema para manejar los errores y recuperarse de ellos satisfactoriamente. La naturaleza del hospedaje en la nube, donde las aplicaciones a menudo son multiinquilino, usan servicios de plataforma compartidos, compiten por los recursos y el ancho de banda, y se ejecutan en hardware estándar, implica que hay una mayor probabilidad de que se produzcan errores transitorios o permanentes. La detección de errores y una recuperación de ellos que sea rápida y eficaz, son necesarias para mantener la resistencia."
keywords: "Patrón de diseño"
author: dragon119
ms.date: 06/23/2017
pnp.series.title: Cloud Design Patterns
ms.openlocfilehash: a3b9d72989e0de57c689bcec51e20653d0441d31
ms.sourcegitcommit: b0482d49aab0526be386837702e7724c61232c60
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/14/2017
---
# <a name="resiliency-patterns"></a>Patrones de resistencia

La resistencia es la capacidad de un sistema para manejar los errores y recuperarse de ellos satisfactoriamente. La naturaleza del hospedaje en la nube, donde las aplicaciones a menudo son multiinquilino, usan servicios de plataforma compartidos, compiten por los recursos y el ancho de banda, y se ejecutan en hardware estándar, implica que hay una mayor probabilidad de que se produzcan errores transitorios o permanentes. La detección de errores y una recuperación de ellos que sea rápida y eficaz, son necesarias para mantener la resistencia.

| Patrón | Resumen |
| ------- | ------- |
| [Bulkhead](../bulkhead.md) | Aísla los elementos de una aplicación en grupos para que si se produce un error en uno, los demás sigan funcionando. |
| [Circuit Breaker](../circuit-breaker.md) | Maneja errores que pueden tardar una cantidad variable de tiempo en solucionarse durante la conexión a un recurso o servicio remoto. |
| [Compensating Transaction](../compensating-transaction.md) | Deshace el trabajo realizado mediante una serie de pasos, que conjuntamente definen una operación definitivamente coherente. |
| [Health Endpoint Monitoring](../health-endpoint-monitoring.md) | Implementa comprobaciones funcionales en una aplicación a la que pueden acceder herramientas externas a través de los puntos de conexión expuestos en intervalos regulares. |
| [Leader Election](../leader-election.md) | Coordina las acciones realizadas por una colección de instancias de tareas de colaboración de una aplicación distribuida mediante la elección de una instancia como líder que asume la responsabilidad de administrar las demás instancias. |
| [Queue-Based Load Leveling](../queue-based-load-leveling.md) | Use una cola que actúe como búfer entre una tarea y un servicio que invoca para equilibrar cargas pesadas intermitentes. |
| [Retry](../retry.md) | Permite que una aplicación trate los errores temporales anticipados cuando intenta conectarse a un servicio o un recurso de red, mediante el reintento de forma transparente de una operación que anteriormente produjo error. |
| [Scheduler Agent Supervisor](../scheduler-agent-supervisor.md) | Coordina un conjunto de acciones en un conjunto distribuido de servicios y otros recursos remotos. |