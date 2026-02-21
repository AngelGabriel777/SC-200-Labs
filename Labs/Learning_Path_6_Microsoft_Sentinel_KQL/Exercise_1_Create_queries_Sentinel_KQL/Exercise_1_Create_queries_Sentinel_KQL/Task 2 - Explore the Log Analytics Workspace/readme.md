# 🧪 TALLER 2  
# Exploración del Log Analytics Workspace en Microsoft Sentinel 

---

## 1. Objetivo

Explorar el Log Analytics Workspace dentro de Microsoft Sentinel, validar el acceso al editor KQL, revisar las tablas disponibles y ejecutar una consulta de prueba para confirmar la visualización de registros.

---

## 2. Entorno de Trabajo

- Portal: https://portal.azure.com  
- Servicio: Microsoft Sentinel  
- Workspace: law-sentinel-lab  
- Interfaz visible: Microsoft Sentinel | Records  

---

## 3. Procedimiento Paso a Paso

---

### 3.1 Acceso al Servicio

1. En la barra de búsqueda del portal Azure escribir:

   Microsoft Sentinel

2. Seleccionar el servicio.
3. Elegir el workspace:

   law-sentinel-lab

4. Verificar que la parte superior muestre:

   Microsoft Sentinel | Records  
   Selected workspace: "law-sentinel-lab"

---

### 3.2 Acceso al Editor de Registros

1. En el panel izquierdo expandir:

   General

2. Seleccionar:

   Records

---

### 3.3 Cierre de Ventanas Emergentes

Si aparecen:

- Ventana emergente de video de Log Analytics → Cerrar.
- Queries hub → Cerrar.

Esto permite trabajar directamente en el editor KQL.

---

### 3.4 Cambio a Modo KQL

1. En la parte superior del editor ubicar el selector de modo.
2. Cambiar de:

   Simple mode

   a

   KQL mode

3. Confirmar que el editor permita escribir consultas manuales.

---

### 3.5 Exploración del Panel de Esquema

En el panel izquierdo observar:

- Lista de tablas disponibles.
- Campos dentro de cada tabla.
- Opciones de filtrado y herramientas adicionales.

En la versión 2026 no se encuentra la tabla:

   SecurityEvent_CL

Debido a que la Microsoft Sentinel Training Lab Solution ya no está disponible.

En su lugar se utilizan tablas estándar como:

- SigninLogs  
- AuditLogs  
- SecurityAlert  
- SecurityIncident  

---

### 3.6 Ejecución de Consulta (Adaptación 2026)

En el editor ingresar la siguiente consulta:

```kql
SigninLogs
| take 1000
