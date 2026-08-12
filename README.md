# RC Solutions — Ecosistema de Automatización IA (Entrega Final, Curso de IA Automation)

Sistema de automatización end-to-end para RC Solutions (instalaciones eléctricas y reparaciones domésticas): desde que un lead completa un formulario de una campaña de Meta hasta que un técnico confirma la visita, con un punto de validación humana (HITL) antes de cualquier confirmación al cliente final.

## Stack

| Categoría | Herramienta |
|---|---|
| Orquestador | n8n |
| Base de datos | Airtable |
| Procesamiento IA | DeepSeek V4-Flash (vía AI Agent) |
| Canales de salida | Slack (HITL + notificaciones), Google Calendar |

## Estructura del repositorio

```
/docs
  Entrega_Final_RC_Solutions_v2.pdf   → Arquitectura, estructuras de datos, matriz de costos, seguridad y resiliencia
/workflow
  Entrega_Final_AI_Automation.json    → Blueprint real de n8n, importable directamente
/screenshots
  (evidencia complementaria, ver nota abajo)
README.md
```

## Enlaces

- **Dashboard de control (Airtable, KPIs):** `https://airtable.com/invite/l?inviteId=inv7kvS43MKHNhm4g&inviteToken=f6f71397ad2a6ea44407f00ef25ae75d2e920ecc0369b29dd4f68d8956d94b94&utm_medium=email&utm_source=product_team&utm_content=transactional-alerts`
- **Base de datos (solo lectura):** `<< https://airtable.com/invite/l?inviteId=inv7kvS43MKHNhm4g&inviteToken=f6f71397ad2a6ea44407f00ef25ae75d2e920ecc0369b29dd4f68d8956d94b94&utm_medium=email&utm_source=product_team&utm_content=transactional-alerts>>`

## Qué muestra el video demo

El video cubre 3 casos ejecutados en vivo sobre el flujo real:
1. **Urgencia** — el lead saltea la clasificación por IA y notifica directo al coordinador.
2. **Electricista (aprobado)** — la IA clasifica el caso, el técnico aprueba por Slack, se crea el evento en Google Calendar.
3. **Pintor (rechazado)** — el técnico rechaza el horario propuesto y coordina la visita por su cuenta; el sistema registra el estado sin intentar reasignar automáticamente.


## Resumen por criterio de evaluación

| Criterio | Dónde está |
|---|---|
| Mapa de arquitectura (20%) | Sección 1 del PDF |
| Estructuras de datos documentadas (20%) | Sección 2 del PDF |
| Optimización de costos (20%) | Sección 3 del PDF |
| Seguridad y resiliencia (20%) | Sección 4 del PDF |
| Dashboard de control (20%) | Sección 5 del PDF + link de Airtable arriba |

---
Rodrigo Crettaz
