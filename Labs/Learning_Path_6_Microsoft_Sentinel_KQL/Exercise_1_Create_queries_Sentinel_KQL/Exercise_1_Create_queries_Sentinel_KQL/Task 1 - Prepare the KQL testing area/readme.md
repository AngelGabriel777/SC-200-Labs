# TALLER 1  
# Preparación del Entorno en Microsoft Sentinel (Interfaz 2026)

---

## 1. Objetivo

Preparar y verificar el entorno de trabajo en Microsoft Sentinel dentro del portal de Microsoft Azure, asegurando que el workspace esté correctamente habilitado y accesible para actividades posteriores.

---

## 2. Entorno de Trabajo

- Plataforma: Microsoft Azure Portal  
- Servicio: Microsoft Sentinel  
- Workspace: law-sentinel-lab  
- Portal: https://portal.azure.com  

---

## 3. Procedimiento

---

### 3.1 Acceso al Portal Azure

1. Abrir el navegador Microsoft Edge.
2. Ingresar a:

   https://portal.azure.com

3. Autenticarse con las credenciales asignadas.
4. Confirmar que el portal cargue correctamente.

---

### 3.2 Acceso a Microsoft Sentinel

1. En la barra de búsqueda superior del portal Azure escribir:

   Microsoft Sentinel

2. Seleccionar el servicio.
3. Elegir el workspace:

   law-sentinel-lab

4. Verificar que la interfaz muestre en la parte superior:

   Microsoft Sentinel | Records  
   Selected workspace: "law-sentinel-lab"

![Acceso a Microsoft Sentinel](images/img1.jpg)

---

### 3.3 Verificación del Workspace

1. Confirmar que el panel lateral muestre las secciones principales del servicio.
2. Validar que el workspace esté activo y sin errores de configuración.

Esta verificación confirma que el servicio se encuentra habilitado correctamente sobre el workspace seleccionado.

---

### 3.4 Acceso al Área de Registros

1. En el menú lateral seleccionar:

   Records

2. Confirmar que se abra el editor de registros (Log Analytics).
3. Verificar que el entorno esté listo para futuras consultas.

![Acceso al área de registros](images/img2.jpg)

---

### 3.5 Verificación de Tablas Disponibles

En el panel izquierdo (Tablas / Schema), confirmar la existencia de tablas activas tales como:

- SigninLogs  
- AuditLogs  
- SecurityAlert  
- SecurityIncident  

La presencia de estas tablas indica que el entorno está correctamente configurado y listo para su utilización en el siguiente taller.

![Verificación de tablas](images/img4.jpg)

---

## 4. Conclusión

Se verificó el acceso al portal Microsoft Azure, la disponibilidad del servicio Microsoft Sentinel y la correcta selección del workspace law-sentinel-lab.  

El entorno quedó preparado y validado para la ejecución de consultas KQL en el Taller 2.
