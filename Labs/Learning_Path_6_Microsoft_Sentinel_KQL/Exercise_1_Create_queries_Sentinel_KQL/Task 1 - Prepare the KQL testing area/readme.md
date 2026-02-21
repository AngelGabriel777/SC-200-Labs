# TALLER 1  
# Preparación y Validación del Entorno en Microsoft Sentinel (Interfaz 2026)

---

## 1. Objetivo

Validar la correcta configuración del entorno de trabajo en Microsoft Sentinel, confirmando:

- Acceso al portal Azure.
- Selección del workspace correcto.
- Disponibilidad de tablas con datos.
- Funcionamiento del editor en modo KQL.
- Ejecución exitosa de consultas.

---

## 2. Entorno de Trabajo

- Workspace: law-sentinel-lab  
- Interfaz: Microsoft Sentinel | Records  
- Portal: https://portal.azure.com  

---

## 3. Procedimiento

---


### 3.2 Acceso al Portal Azure

1. Abrir Microsoft Edge.
2. Ingresar a:

   https://portal.azure.com

3. Autenticarse con las credenciales asignadas.
4. Verificar carga exitosa del portal.

---

### 3.3 Acceso a Microsoft Sentinel

1. En la barra de búsqueda superior escribir:

   Microsoft Sentinel

2. Seleccionar el servicio.
3. Elegir el workspace:

   law-sentinel-lab

4. Confirmar que la interfaz muestre en la parte superior:

   Microsoft Sentinel | Records  
   Selected workspace: "law-sentinel-lab"
   
![Descripción de la imagen](images/img1.jpg)

---


### 3.5 Acceso al Editor de Consultas

1. En el menú izquierdo seleccionar:

   Records

2. Confirmar que el editor esté configurado en:

   Modo KQL

3. Si aparece "Modo simple", cambiar manualmente a Modo KQL.

![Descripción de la imagen](images/img2.jpg)

---

### 3.6 Verificación de Tablas

En el panel izquierdo del editor revisar la sección Tablas y confirmar la existencia de:

- SigninLogs  
- AuditLogs  
- SecurityAlert  
- SecurityIncident  

![Descripción de la imagen](images/img4.jpg)

---

### 3.7 Validación de Datos

En el editor KQL ejecutar la siguiente consulta:

```kql
SigninLogs
| take 10
```

![Descripción de la imagen](images/img3.jpg)



