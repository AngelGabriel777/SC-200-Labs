# 🛡️ Lab 1 – Enable Microsoft Defender for Cloud  
**Learning Path 5 – Mitigate threats using Microsoft Defender for Cloud**

Este laboratorio forma parte del portafolio del curso **SC-200**.  
El objetivo es **habilitar Microsoft Defender for Cloud**, conectar un servidor híbrido mediante **Azure Arc**, habilitar los planes de protección y revisar la postura de seguridad desde el portal.

---

# 🎯 Objetivos del Laboratorio

1. Conectar un servidor local (Windows Server) preconfigurado con Azure Arc.  
2. Habilitar Microsoft Defender for Cloud:  
   - CSPM (Cloud Security Posture Management)  
   - Servidores Plan 2 (Cloud Workload Protection)  
3. Revisar el panel de Microsoft Defender for Cloud y comprender cada componente.

---

# 🧩 Escenario

Actúo como **Security Operations Analyst**.  
La empresa está implementando protecciones de cargas de trabajo en la nube mediante Microsoft Defender for Cloud.  
Mi objetivo es conectar un servidor local → habilitar Defender → revisar la postura de seguridad.

---

# 🏁 Prerrequisitos del laboratorio

- Servidor local con Azure Arc preinstalado → *WINServer*  
- Máquina remota Windows para administrar Azure → *WIN1*  
- Acceso a Azure Portal  
- Suscripción de laboratorio (MOC Subscription)  
- Credenciales del tenant del laboratorio

---

# ✅ Tarea 1 – Conectar un servidor local mediante Azure Arc

### 📌 1. Ingreso al servidor WINServer  
- Inicio sesión en **WINServer** como administrador.  
- Confirmo que Azure Arc ya está preinstalado.

### 📌 2. Ejecutar el comando de conexión  
Abrí **cmd como administrador** y ejecuté:

```powershell
azcmagent connect -g "defender-RG" -l "EastUS" -s "<Subscription-ID>"
