# 📄 Informe Técnico – Taller 6: Checklist de Cumplimiento Normativo

## 🔖 Nombre del Taller
_Taller 6 – Checklist de Cumplimiento Normativo: Habeas Data, ISO/IEC 27001 y Protección de Datos Personales_

---

## 👥 Integrantes del equipo
- Isabela Díaz Acosta 
- Samuel Esteban López Huertas 
- Sebastián Sánchez Sandoval 

---

## 🧠 Descripción general del trabajo

El objetivo del taller fue verificar los aspectos legales, normativos y de cumplimiento aplicables a un sistema de información, utilizando listas de control basadas en los marcos: **Ley 1581 de 2012 (Habeas Data)**, **ISO/IEC 27001** y principios generales de **protección de datos personales en Colombia**.

La actividad se desarrolló en dos fases:

1. **Parte 1 – Caso base (GobData):** Se aplicó el checklist al portal estatal ficticio GobData, un sistema de trámites ciudadanos que procesa datos sensibles como historial médico, antecedentes, identificaciones y certificados digitales. Esta fase permitió al equipo familiarizarse con la lógica normativa de cada criterio y desarrollar criterio para justificar los niveles de cumplimiento.

2. **Parte 2 – Cliente real (Falek Latina S.A.S.):** Se trasladó la misma metodología al sistema de información de **Falek Latina S.A.S.**, empresa colombiana con más de 40 años de experiencia en la comercialización de insumos y equipos para fundición, con operaciones en Colombia, Latinoamérica y EE.UU. La evaluación se realizó con base en información pública disponible (sitio web, registros empresariales, objeto social y comunicaciones corporativas).

---

## 🔧 Proceso de desarrollo

El equipo siguió el siguiente proceso:

1. **Lectura y análisis del caso GobData:** Se revisó el enunciado del taller y se identificaron las secciones del checklist: Consentimiento Informado, Habeas Data (Ley 1581), Seguridad (ISO 27001), Retención y Eliminación, Auditoría y Trazabilidad, Terceros y Encargados, y Transferencia Internacional.

2. **Diligenciamiento del checklist caso base:** Para cada uno de los 20 criterios del checklist GobData se asignó un nivel de cumplimiento (✅ Cumple / ⚠️ Parcial / ❌ No cumple), se redactó la evidencia o justificación técnica y se propuso una recomendación accionable.

3. **Identificación de brechas:** A partir de los criterios con ⚠️ y ❌, se consolidó la hoja de *Brechas y Riesgos*, describiendo el impacto de cada brecha y su nivel de prioridad (Alta, Media, Baja).

4. **Aplicación al cliente real (Falek Latina):** Se adaptó la misma estructura del checklist al perfil de Falek Latina, ampliando el análisis con categorías relevantes para su sector (comercio exterior, ISO 9001, SAGRILAFT, transporte de mercancías peligrosas). Los hallazgos se basaron en fuentes públicas disponibles y se documentaron con justificación técnica y legal.

5. **Investigación complementaria:** Se profundizó en las normativas aplicables en Colombia y se consultaron fuentes oficiales (SIC, MinTIC, ICONTEC) para fundamentar las recomendaciones.

**Herramientas utilizadas:** Microsoft Excel (para el checklist), Markdown (para el informe y notas), información pública de Falek Latina (faleklatina.com, EMIS, Cámara de Comercio de Bogotá).

---

## 🧩 Análisis del modelo propuesto

### Estructura del checklist entregado

El checklist se organiza en dos hojas de trabajo:

- **Checklist de Cumplimiento:** 20 criterios (caso GobData) + criterios adicionales (cliente real), organizados en 7 categorías normativas, con campos de nivel de cumplimiento, evidencia/justificación y recomendación.
- **Brechas y Riesgos:** Registro consolidado de las brechas identificadas, con descripción del riesgo, recomendación prioritaria y nivel de prioridad (Alta / Media / Baja).

### Cómo representa las necesidades del cliente

Para **GobData**, el checklist refleja los riesgos propios de una plataforma estatal que procesa datos sensibles de ciudadanos: la ausencia de mecanismos de revocación de consentimiento, la falta de cifrado en reposo y la inexistencia de una política de retención de datos son brechas de alto impacto que podrían derivar en sanciones de la SIC y pérdida de confianza ciudadana.

Para **Falek Latina**, el checklist adapta los criterios al perfil de una empresa distribuidora B2B de 13 empleados con operaciones de comercio exterior. Las brechas más relevantes se concentran en: ausencia de política de seguridad de la información (ISO 27001), incumplimientos de la Ley 1581 en el sitio web (formulario de contacto sin consentimiento explícito) y la falta de canales habilitados para derechos ARCO.

### Supuestos tomados

- Los niveles de cumplimiento del caso GobData corresponden al escenario ficticio provisto por la plantilla del taller.
- Para Falek Latina, todos los niveles de cumplimiento se basan exclusivamente en información pública disponible. Los criterios marcados como ❌ podrían estar cubiertos internamente sin evidencia pública.
- Se asume que Falek Latina no tiene certificación ISO 27001 dado que no se anuncia en ningún canal corporativo.
- Se asume que la ISO en proceso es ISO 9001:2015 (Gestión de Calidad), que es la más referenciada en su sector industrial.

---

## 📈 Checklist y brechas entregados

> Los archivos `checklist-gobdata.xlsx` (caso base GobData) y `checklist-cliente.xlsx` (Falek Latina S.A.S.) se encuentran en la carpeta `clase/` y `entrega/` del repositorio respectivamente.

**Resumen de resultados – Caso Base GobData:**

| Categoría | ✅ Cumple | ⚠️ Parcial | ❌ No cumple |
|---|:---:|:---:|:---:|
| Consentimiento Informado | 1 | 1 | 1 |
| Habeas Data – Ley 1581 | 2 | 1 | 0 |
| Seguridad – ISO 27001 | 3 | 2 | 0 |
| Retención y Eliminación | 0 | 0 | 2 |
| Auditoría y Trazabilidad | 1 | 1 | 0 |
| Terceros y Encargados | 1 | 1 | 0 |
| Transferencia Internacional | 0 | 1 | 0 |

**Resumen de resultados – Cliente Real (Falek Latina S.A.S.):**

| Categoría | ✅ | ⚠️ | ❌ |
|---|:---:|:---:|:---:|
| ISO 9001 – Gestión de Calidad | 2 | 5 | 0 |
| ISO 27001 – Seguridad de la Información | 0 | 2 | 5 |
| Ley 1581 / Habeas Data | 0 | 3 | 4 |
| GDPR (evaluación de alcance) | 0 | 1 | 2 |
| Comercio Exterior / Regulatorio | 2 | 2 | 0 |

---

## 📋 Tabla de actores, entidades o componentes

| Nombre del elemento | Tipo | Descripción | Relevancia normativa |
|---|---|---|---|
| Ciudadano / Titular | Actor | Usuario que realiza trámites en GobData y cuyos datos son tratados | Titular de derechos ARCO (Ley 1581, Art. 8) |
| Funcionario público | Actor | Empleado que accede y gestiona los datos de los ciudadanos | Sujeto a control de acceso RBAC (ISO 27001, A.9) |
| Responsable de Tratamiento | Rol | Entidad pública que determina los fines y medios del tratamiento de datos | Obligación legal Ley 1581, Art. 17 |
| Encargado del Tratamiento | Rol | Proveedor de nube/hosting que procesa datos por cuenta de GobData | Debe tener cláusulas contractuales de protección de datos (Ley 1581, Art. 18) |
| SIC | Entidad de control | Superintendencia de Industria y Comercio, autoridad de datos personales en Colombia | Receptora de declaraciones, registros de BD y quejas de titulares |
| MinTIC | Entidad reguladora | Ministerio de Tecnologías de la Información – emite lineamientos de seguridad digital para el Estado | Marco de Seguridad Digital del Estado Colombiano |
| Módulo de historial clínico | Sistema | Componente de GobData que almacena datos de salud (datos sensibles) | Sujeto a controles adicionales: Art. 6 Ley 1581, cifrado en reposo |
| Proveedor de nube | Sistema/Tercero | Infraestructura en EE.UU. y España donde se replican datos | Transferencia internacional de datos: Art. 26 Ley 1581 |
| Falek Latina S.A.S. | Cliente real | Empresa distribuidora de insumos para fundición con operaciones en Colombia, LatAm y EE.UU. | Responsable del tratamiento de datos de clientes y contactos comerciales |

---

## 🔍 Investigación complementaria

### Tema investigado:
Normativas colombianas de protección de datos personales (Ley 1581 de 2012 y Decreto 1377 de 2013), ISO/IEC 27001:2022 como estándar de gestión de seguridad de la información, y normativas sectoriales aplicables a empresas de comercio exterior en Colombia (SAGRILAFT, Decreto 1609/2002).

### Resumen:

**Ley 1581 de 2012 – Habeas Data (Colombia):** Esta ley establece el marco general de protección de datos personales en Colombia, definiendo los derechos de los titulares (acceso, corrección, supresión, revocación y queja), las obligaciones de los responsables y encargados del tratamiento, y el régimen sancionatorio a cargo de la SIC. El Decreto 1377 de 2013 la reglamenta en aspectos como la autorización de tratamiento, las políticas de privacidad y la figura del Encargado. Para GobData, la Ley 1581 es la normativa de mayor impacto dado el volumen y sensibilidad de los datos ciudadanos tratados. Para Falek Latina, aplica especialmente a los datos de clientes, contactos comerciales y empleados.

**ISO/IEC 27001:2022 – Gestión de Seguridad de la Información:** Este estándar internacional establece los requisitos para implementar, mantener y mejorar un Sistema de Gestión de Seguridad de la Información (SGSI). Su versión 2022 actualiza los controles del Anexo A a 93 controles en 4 dominios (organizacional, personas, físico y tecnológico). Es especialmente relevante para GobData por el volumen de datos sensibles que procesa. Para Falek Latina, aunque no tiene certificación ISO 27001, los controles mínimos del estándar (política de SI, gestión de accesos, backups cifrados, gestión de incidentes) son aplicables como buenas prácticas y serán exigidos por sus clientes corporativos a medida que la empresa crece.

**Normativas sectoriales (Falek Latina):** La empresa está sujeta a regulaciones adicionales por su actividad de comercio exterior: el **SAGRILAFT** (Sistema de Autocontrol y Gestión del Riesgo de Lavado de Activos) para operaciones con países de riesgo como Venezuela; el **Decreto 1609 de 2002** sobre transporte de mercancías peligrosas (relevante para insumos químicos de fundición); y las obligaciones ante la **DIAN** en materia de importación/exportación. En materia de calidad, se encuentra en proceso de certificación **ISO 9001:2015**, lo que evidencia una madurez incipiente en gestión de procesos, aunque todavía no se extiende a la seguridad de la información.

---

## 📚 Referencias

Ver archivo `referencias.md` en la carpeta `entrega/` del repositorio para el listado completo de fuentes.

---

_Este documento hace parte de la entrega del Taller 6 del curso AREM (Arquitectura Empresarial) – Universidad de La Sabana._

