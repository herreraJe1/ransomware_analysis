# 🛡️ Informe Técnico – Ransomware Conti (2022)

## 1. Introducción

Conti fue una de las variantes de ransomware más activas y sofisticadas entre 2020 y 2022. Operaba bajo el modelo Ransomware-as-a-Service (RaaS), permitiendo que afiliados ejecutaran ataques coordinados. En 2022, su código fuente fue filtrado, lo que permitió a investigadores analizar sus tácticas, pero también facilitó la creación de variantes por otros actores maliciosos.

## 2. Funcionamiento general

- Cifrado rápido de archivos sensibles
- Exfiltración de datos confidenciales
- Doble extorsión: bloqueo + amenaza de filtración
- Uso de infraestructura distribuida para evasión

## 3. Vectores de ataque

### Entrada inicial

- Correos de phishing con documentos maliciosos
- Explotación de vulnerabilidades RDP
- Uso de malware auxiliar como TrickBot y Zloader

### Escalamiento y persistencia

- Robo de credenciales con Mimikatz
- Modificación de claves del registro
- Tareas programadas y cuentas locales
- Uso de PsExec y PowerShell para movimientos laterales

### Cifrado y extorsión

- Archivos cifrados con extensiones como `.conti`, `.crypt`
- Nota de rescate con instrucciones de pago
- Amenaza de publicación de datos si no se paga

## 4. Recursos de análisis

- Artículos:  
  - *Understanding Ransomware Trends*  
  - *Conti: Ransomware Analysis*

- Videos educativos:  
  - *Conti | TryHackMe | Walkthrough*  
  - *Analyzing Conti Ransomware*  
  - *Conti Ransomware Gang Analysis*

- Código fuente:  
  - GitHub: *Ransomware Simulator*

## 5. Medidas de protección

### Prevención

- Capacitación en ciberseguridad y phishing
- Actualización constante de sistemas
- Autenticación multifactor (MFA)

### Respuesta

- Copias de seguridad fuera de línea
- Segmentación de red
- Soluciones EDR para detección avanzada

### Recuperación

- Plan de recuperación ante desastres
- Evaluación periódica de impacto potencial
