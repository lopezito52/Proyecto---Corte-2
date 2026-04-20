# Proyecto---Corte-2
# 🏛️ Arquitectura Empresarial — Talleres Corte 2
 
> Repositorio académico del equipo conformado por **Isabela Díaz Acosta**, **Samuel Esteban López Huertas** y **Sebastián Sánchez Sandoval**.  
> Materia: **Arquitectura Empresarial** · Universidad de la Sabana· 2026
 
---
 
## 📁 Estructura del repositorio
 
```
Proyecto corte 2/
├── TALLER4/
│   ├── informe.md
│   ├── referencias.md
│   └── Mapa-Final
├── TALLER5/
│   ├── informe_taller.md
│   ├── referencias.md
│   └── tabla_stride_cliente_final
└── TALLER6/
    ├── informe.md
    ├── referencias.md
    └── checklist-gobdata_FalekLatna.xlsx 
```
 
---
 
## 👥 Integrantes del equipo
 
| Nombre | Rol |
|---|---|
| Isabela Díaz Acosta | Investigación y análisis normativo |
| Samuel Esteban López Huertas | Modelamiento y documentación técnica |
| Sebastián Sánchez Sandoval | Diagramación y arquitectura de sistemas |
 
---
 
## 📚 Descripción de los talleres
 
### 🗺️ Taller 4 — Mapa de Infraestructura y Diagnóstico Técnico
 
Modelamiento de la infraestructura tecnológica **AS-IS** de una organización con presencia en tres sedes (Bogotá, Cota y Barranquilla). El trabajo consistió en:
 
- Auditoría y mapeo visual de la topología de red híbrida (On-Premise + Cloud).
- Identificación de **Puntos Únicos de Falla (SPOF)**, especialmente la dependencia crítica del servidor local en Bogotá.
- Análisis de escalabilidad considerando el uso de Google Drive como capa de persistencia.
- Propuesta de migración hacia arquitectura **Cloud-Native** para garantizar alta disponibilidad.
**Tecnologías y conceptos clave:** infraestructura híbrida, WAN/VPN, alta disponibilidad, SPOF, SaaS.
 
---
 
### 🔐 Taller 5 — Evaluación de Seguridad con STRIDE
 
Análisis de seguridad de sistemas empresariales aplicando el modelo **STRIDE** (Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, Elevation of Privilege). Se trabajaron dos contextos:
 
- **Caso base – EdukIT:** flujos críticos de un sistema educativo.
- **Caso real – Proceso de cotización y venta del cliente:** identificación de amenazas en el ciclo comercial (cliente → asesor → sistema → inventario → contabilidad).
Los puntos críticos identificados fueron el **manejo del inventario** y la **validación de cotizaciones**, por su impacto directo en ingresos y reputación.
 
**Tecnologías y conceptos clave:** STRIDE, modelado de amenazas, OWASP, autenticación multifactor, cifrado, control de accesos.
 
---
 
### ✅ Taller 6 — Checklist de Cumplimiento Normativo
 
Verificación de cumplimiento legal y normativo de sistemas de información bajo tres marcos regulatorios:
 
| Marco | Descripción |
|---|---|
| **Ley 1581 de 2012** | Habeas Data y protección de datos personales en Colombia |
| **ISO/IEC 27001:2022** | Gestión de Seguridad de la Información |
| **GDPR / Normativas sectoriales** | Comercio exterior, SAGRILAFT, Decreto 1609/2002 |
 
Se evaluaron dos casos:
- **GobData** (caso base ficticio): portal estatal de trámites ciudadanos con datos sensibles.
- **Falek Latina S.A.S.** (cliente real): empresa distribuidora de insumos para fundición con operaciones en Colombia, LatAm y EE.UU.
**Resultado destacado:** Falek Latina presentó brechas críticas en ISO 27001 y Ley 1581, incluyendo ausencia de política de seguridad de la información y falta de mecanismos para derechos ARCO.
 
---
### Presentacion Falek Latina Infraestructura - SEGURIDAD - NORMATIVA
- https://www.canva.com/design/DAHHK2m2zJE/4AD5l8AlU8UjgXjN-l44zA/edit

## 🔗 Recursos y referencias
 
Cada carpeta de taller contiene un archivo `referencias.md` con las fuentes utilizadas. Entre las principales:
 
- [OWASP Foundation](https://owasp.org)
- [Microsoft — STRIDE Threat Model](https://learn.microsoft.com/en-us/azure/security/develop/threat-modeling-tool-threats)
- [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework)
- [SIC — Superintendencia de Industria y Comercio](https://www.sic.gov.co)
- [MinTIC — Marco de Seguridad Digital](https://www.mintic.gov.co)
- ISO/IEC 27001:2022 — ICONTEC / ISO
