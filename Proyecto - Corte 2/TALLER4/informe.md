# 📄 Informe Técnico del Taller

## 🔖 Nombre del Taller
_Taller 4 - Mapa de Infraestructura y Diagnóstico Técnico_

## 👥 Integrantes del equipo
- Sebastian Sanchez Sandoval
- Isabela Diaz
- Samuel Esteban Lopez Huertas

## 🧠 Descripción general del trabajo
El objetivo de este taller consistió en el modelamiento de la infraestructura tecnológica "AS-IS" y la identificación de puntos críticos de falla. Se analizó una topología híbrida que interconecta tres sedes geográficas (Bogotá, Cota y Barranquilla), evaluando la dependencia de servidores locales y servicios en la nube para la gestión de procesos logísticos.

## 🔧 Proceso de desarrollo
1.  **Auditoría de Red:** Se examinó la representación visual de la infraestructura, identificando los nodos de red (routers/switches) y los flujos de datos.
2.  **Mapeo de Terminales:** Se categorizaron los tipos de estaciones (Asesor, Gerente, Contador, Logística) y su método de acceso a los recursos centrales.
3.  **Detección de Riesgos Técnicos:** Se analizaron las rutas de conexión, identificando la dependencia crítica del servidor local en Bogotá para el funcionamiento de las sedes remotas.
4.  **Análisis de Escalabilidad:** Se evaluó el uso de Google Drive como solución de persistencia de datos frente a la carga operativa de las sedes regionales.

## 🧩 Análisis del modelo propuesto
- **Estructura Híbrida:** El sistema combina activos locales (On-Premise) en la sede principal con almacenamiento en la nube (SaaS - Google Drive).
- **Necesidades del Cliente:** El modelo refleja una operación distribuida donde Cota y Barranquilla dependen de la conectividad WAN para sincronizar información con el servidor central.
- **Supuestos Técnicos:**
    - El "Servidor Local" en Bogotá centraliza la lógica de negocio y bases de datos.
    - Las sedes regionales se conectan a través de Internet pública, posiblemente mediante túneles VPN.
    - No existe redundancia física para el servidor principal ni para los enlaces de salida a Internet en las sedes.

## 📈 Diagrama final entregado
![Mapa de Infraestructura](./clase/mapa-borrador.drawio.png)

## 📋 Tabla de componentes de infraestructura

| Nombre del elemento | Tipo | Descripción | Responsable |
|---------------------|------|-------------|-------------|
| Servidor Local      | Hardware | Nodo central de procesamiento y datos en Bogotá. | TI Interna |
| Google Drive        | Cloud SaaS | Repositorio en la nube para persistencia de archivos compartidos. | Google |
| Router/Switch (BOG) | Network | Core de red que gestiona el tráfico interno y salida a WAN. | TI / ISP |
| Estación Logística  | Endpoint | Terminales para el registro de procesos operativos regionales. | Operarios |
| Routers Regionales  | Network | Puntos de borde que permiten la conectividad de Cota y B/quilla. | ISP |

## 🔍 Investigación complementaria
### Tema investigado:
**Puntos Únicos de Falla (SPOF) y Alta Disponibilidad en Redes Distribuidas.**

### Resumen:
El diagnóstico técnico revela que la infraestructura actual posee un **Punto Único de Falla (SPOF)** crítico en el Servidor Local de Bogotá. Si este hardware o su enlace de red fallan, las sedes de Cota y Barranquilla pierden capacidad de operación. Basado en las buenas prácticas de arquitectura de alta disponibilidad, se recomienda la migración hacia una arquitectura **Cloud-Native**.

La implementación de servicios de base de datos distribuidos y un **API Gateway** en la nube permitiría que las sedes regionales operen de forma independiente a la infraestructura física de Bogotá. Esto reduce la latencia de red y garantiza la continuidad del negocio mediante la eliminación de dependencias geográficas centralizadas.