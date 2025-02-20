# Chaos Engineering en AWS
## 🌟 Introducción
- Chaos Engineering es la práctica de experimentar en un sistema distribuido para identificar debilidades antes de que ocurran fallas reales. 
- Este enfoque permite mejorar la resiliencia de tus aplicaciones en AWS al probar cómo responden tus sistemas ante fallos inesperados.

## 🔍 Objetivos de Chaos Engineering
- Identificar puntos débiles en arquitecturas resilientes.
- Validar estrategias de recuperación ante desastres y alta disponibilidad.
- Asegurar que los sistemas puedan recuperarse rápidamente frente a incidentes como fallas de red, pérdida de instancias, o interrupciones de servicios.

## 🛠️ Herramientas y servicios relacionados en AWS
AWS ofrece varias herramientas y servicios que pueden facilitar la implementación de Chaos Engineering:
1. **AWS Fault Injection Simulator (FIS)**
    - Permite realizar experimentos controlados de falla en servicios como EC2, RDS, y EKS.
    - Ejemplo: Simular la detención de instancias de EC2 para verificar la efectividad de Auto Scaling.
2. AWS CloudWatch
    - Supervisa métricas y alarmas durante las pruebas de Chaos Engineering para validar el comportamiento esperado.
3. AWS Systems Manager
    - Automatiza experimentos en tus entornos mediante ejecuciones planificadas.
4. Integraciones con Herramientas Externas
    - Herramientas como Gremlin o Chaos Monkey de Netflix pueden complementarse con AWS para pruebas más avanzadas.

## 🧰 Herramientas adicionales de Chaos Engineering
Además de AWS Fault Injection Simulator (FIS), existen otras herramientas populares que se utilizan en el ámbito de Chaos Engineering. Algunas de ellas son:
1. Chaos Monkey
    - Chaos Monkey es parte del conjunto de herramientas de **Simian Army** creado por Netflix. Su función es aleatoriamente eliminar instancias de servidores para probar la resiliencia del sistema.
    - Es particularmente útil para aplicaciones distribuidas en la nube, como las que se ejecutan en AWS.
2. Gremlin
    - Gremlin ofrece una plataforma más robusta para realizar experimentos de Chaos Engineering. 
    - Permite crear fallas controladas en tus servicios y ofrece soporte para AWS, GCP, y otros entornos.
3. Chaos Toolkit
    - Es una herramienta de código abierto que permite la creación y ejecución de experimentos de Chaos Engineering integrándose con plataformas como AWS, Kubernetes y más.
4. LitmusChaos
    - LitmusChaos es una plataforma de Chaos Engineering basada en Kubernetes, que se puede integrar en entornos que usen Amazon EKS.

## 🚀 Pasos para Implementar Chaos Engineering en AWS
1. Define el Experimento
    - Determina qué componente del sistema deseas probar y qué métrica usarás para medir el éxito (por ejemplo, tiempo de recuperación).
2. Introduce Fallas Controladas
    - Utiliza AWS FIS para simular interrupciones, como pérdida de red, sobrecarga de CPU o reinicio de instancias.
3. Observa y Analiza
    - Monitorea el impacto con CloudWatch y verifica que los mecanismos de resiliencia (como Auto Scaling o failover) respondan según lo esperado.
4. Aprende y Mejora
    - Ajusta la arquitectura o configura alarmas adicionales basadas en los resultados obtenidos.

### 🔗 Enlaces útiles
- [¿Qué es la ingeniería del caos?](https://www.ibm.com/mx-es/think/topics/chaos-engineering)
- [AWS Fault Injection Simulator (FIS) - Documentación Oficial](https://aws.amazon.com/es/fis/)
- [Introducción a Chaos Engineering en AWS](https://aws.amazon.com/es/solutions/resilience/chaos-engineering/)
- [Chaos Engineering on AWS](https://aws.amazon.com/es/blogs/architecture/chaos-engineering-in-the-cloud/)
- [Gremlin - Chaos Engineering Platform](https://www.gremlin.com/)
- [Chaos Monkey en GitHub](https://github.com/Netflix/chaosmonkey)
- [Chaos Toolkit](https://chaostoolkit.org/)
- [LitmusChaos](https://litmuschaos.io/)