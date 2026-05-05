# integracion-escolar-2026
Automatización de notificaciones a familias- Integración Escolar 2026 - Google Apps Script
# 🏫 Sistema de Notificaciones - Integración Escolar 2026
**Assistire - Centro de Rehabilitación Integral (Centro)**

Script desarrollado en Google Apps Script para automatizar el envío de emails a padres de pacientes con tratamiento de Integración Escolar / Asistente Externo 2026 autorizado, adjuntando el instructivo oficial en PDF desde Google Drive.

---

## ⚙️ Archivos del proyecto

| Archivo | Función |
|---|---|
| `Script integracion escolar.txt` | Script principal de envío de emails a padres |

---

## 🚀 Funcionalidades

- Envío individual desde la fila seleccionada o masivo de todos los pendientes
- Validación robusta de emails reales: descarta placeholders como `"E-MAIL"`, `"E mail"`, `"E_mail"`
- Adjunta PDF institucional desde Google Drive con fallback por normalización de espacios
- Doble menú accesible: desde **Extensiones** y desde la barra superior de Google Sheets
- Indicadores visuales por celda: 🟡 amarillo durante envío, 🔴 rojo si email inválido
- Registro automático de fecha de envío en columna G (evita duplicados)
- Trigger instalable `onOpen` para activación persistente al abrir el documento

---

## 📧 Flujo del sistema
Hoja "Casos Aprobados"
↓
Validar email real en col F
↓
Enviar email con PDF adjunto
↓
Registrar fecha en col G ✅


---

## 🛠️ Stack

`Google Apps Script` · `GmailApp` · `DriveApp` · `HTML email` · `ScriptApp Triggers`

---

## 👤 Autor
Iván De la torre — [GitHub](https://github.com/Delatorreivan1998)
