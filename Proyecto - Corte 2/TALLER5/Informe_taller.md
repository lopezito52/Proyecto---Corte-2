# 📄 `Informe`

## 🔖 Nombre del Taller

Taller 5 - Evaluación de Seguridad con STRIDE

## 👥 Integrantes del equipo

Isabela Díaz Acosta
Sebastián Sánchez Sandoval
Samuel Esteban López Huertas

## 🧠 Descripción general del trabajo

El objetivo de este taller fue analizar la seguridad de sistemas mediante el modelo STRIDE, identificando amenazas potenciales en procesos críticos y proponiendo estrategias de mitigación. Se trabajó en dos contextos: un caso base (EdukIT) y un caso real del cliente (proceso de cotización y venta).

## 🔧 Proceso de desarrollo

El equipo inició seleccionando los flujos críticos de ambos sistemas. Posteriormente, se identificaron los componentes clave (usuarios, sistemas, bases de datos, etc.) y se aplicó el modelo STRIDE a cada uno.

Se utilizó:

* Excel para estructurar amenazas
* Análisis lógico basado en arquitectura del sistema

Se priorizaron amenazas según impacto en negocio (ventas, datos, operación).

## 🧩 Análisis del modelo propuesto

El modelo de cotización representa un flujo completo desde la solicitud del cliente hasta el registro contable.

Refleja correctamente:

* Interacción entre áreas (comercial, sistema, contable)
* Dependencia del inventario
* Punto crítico de conversión (aceptación)

Supuestos:

* Inventario en tiempo real
* Integración CRM–contable
* Usuario responde oportunamente

## 📈 Diagrama final entregado

El excel está adjunto en la carpeta

## 📋 Tabla de componentes

| Nombre       | Tipo    | Descripción         | Responsable |
| ------------ | ------- | ------------------- | ----------- |
| Cliente      | Actor   | Solicita cotización | Cliente     |
| Asesor       | Actor   | Genera cotización   | Comercial   |
| Sistema      | Sistema | Valida y procesa    | TI          |
| Inventario   | Datos   | Control de stock    | Operaciones |
| Contabilidad | Sistema | Registra ventas     | Finanzas    |

---

## 🔍 Investigación complementaria

### Tema investigado:

Seguridad en sistemas empresariales y modelo STRIDE

### Resumen:

El modelo STRIDE permite clasificar amenazas en seis categorías clave: suplantación, manipulación, repudio, divulgación, denegación de servicio y elevación de privilegios. Este enfoque facilita identificar vulnerabilidades en sistemas distribuidos.

En contextos empresariales como ventas o educación, es fundamental implementar controles como autenticación multifactor, cifrado de datos, control de accesos y monitoreo de logs. Estas prácticas reducen riesgos asociados a fraude, filtración de información y fallos operativos.

En el caso del cliente, se evidenció que los puntos más críticos son el manejo del inventario y la validación de cotizaciones, ya que impactan directamente en ingresos y reputación.

---

## 📚 Referencias

* OWASP Foundation. *OWASP Top 10*. [https://owasp.org](https://owasp.org)
* Microsoft. *STRIDE Threat Model*.
* NIST. *Cybersecurity Framework*.
* Fuente asistida por IA: ChatGPT, 2026


