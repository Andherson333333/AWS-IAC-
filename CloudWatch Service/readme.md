## Índice de contenidos
* [¿Qué es AWS CloudWatch?](#item1)
* [¿Qué es una alarma?](#item2)
* [¿Qué es una métrica?](#item3)
* [¿Qué son los logs?](#item4)
* [¿Qué son los X-Ray traces?](#item5)
* [¿Qué es un evento?](#item6)
* [¿Qué es Application Signal?](#item7)
* [¿Qué es Network Monitoring?](#item8)
* [¿Qué son los Insights?](#item9)
* [Configuración de cloudwathc con IAC](#item10)

<a name="item1"></a>
## ¿Qué es AWS CloudWatch?

AWS CloudWatch es un servicio de monitoreo y observabilidad de Amazon Web Services (AWS) que te permite recopilar, monitorizar y analizar métricas, logs y eventos para obtener una visión completa de tus recursos y aplicaciones en la nube.

<a name="item2"></a>
## ¿Qué es una alarma?

Una alarma en CloudWatch te permite monitorear una métrica específica y realizar acciones automáticamente cuando la métrica cumple ciertos criterios. Las alarmas pueden enviar notificaciones, activar acciones de Auto Scaling o ejecutar funciones de Lambda.

<a name="item3"></a>
## ¿Qué es una métrica?

Una métrica es un dato representativo que indica el rendimiento de un recurso. CloudWatch recopila métricas de muchos servicios de AWS (como EC2, RDS, S3) y te permite definir y enviar tus propias métricas personalizadas.

<a name="item4"></a>
## ¿Qué son los logs?

Los logs en CloudWatch Logs te permiten recopilar, monitorizar y analizar los registros de tus aplicaciones y servicios. Puedes crear métricas basadas en patrones de logs y realizar consultas para obtener información detallada sobre el comportamiento de tus aplicaciones.

<a name="item5"></a>
## ¿Qué son los X-Ray traces?

AWS X-Ray es un servicio que te permite analizar y depurar aplicaciones distribuidas. Traces son registros de todas las solicitudes que recorren los servicios en tu aplicación, proporcionando una visión detallada del flujo de solicitudes y la latencia en cada componente.

<a name="item6"></a>
## ¿Qué es un evento?

CloudWatch Events (ahora parte de Amazon EventBridge) permite reaccionar a cambios en tu entorno AWS casi en tiempo real. Puedes configurar reglas que detecten eventos operacionales y activen acciones como invocar funciones de Lambda o enviar notificaciones.

<a name="item7"></a>
## ¿Qué es Application Signal?

Application Signals son indicadores de la salud y el rendimiento de una aplicación. En el contexto de CloudWatch, puedes monitorear señales como métricas de rendimiento, logs de aplicaciones y trazas de X-Ray para obtener una vista completa del estado de tu aplicación.

<a name="item8"></a>
## ¿Qué es Network Monitoring?

Network Monitoring en CloudWatch te permite monitorear y diagnosticar problemas de red en tus recursos de AWS. Puedes utilizar métricas de red de servicios como VPC, CloudFront y ELB para obtener información sobre el tráfico y la latencia.

<a name="item9"></a>
## ¿Qué son los Insights?

CloudWatch Insights proporciona herramientas para realizar consultas avanzadas y análisis en logs y métricas. Log Insights permite buscar y analizar grandes volúmenes de logs rápidamente, mientras que Metric Insights te ayuda a identificar patrones y tendencias en las métricas.

<a name="item10"></a>
## Configuración de cloudwathc con IAC

Este repositorio incluye la configuración de Terraform y cloduformation que crea los siguientes recursos:
- Una alarma de CloudWatch para monitorear la utilización de CPU de una instancia EC2 específica.
- Un tema SNS y una suscripción de correo electrónico para recibir notificaciones.
- Un dashboard de CloudWatch para visualizar las métricas.


![Diagrama](https://github.com/Andherson333333/AWS-IAC/blob/main/CloudWatch%20Service/imagenes/cloudwatch.png)

![Diagrama](https://github.com/Andherson333333/AWS-IAC/blob/main/CloudWatch%20Service/imagenes/cloudwatch-1.png)

