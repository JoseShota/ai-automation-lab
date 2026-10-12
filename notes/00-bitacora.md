# Bitácora

Una entrada por sesión. Formato: qué hice, qué aprendí, qué sigue, horas.

---

## 2026-10-12 (lunes) · Arranque

**Objetivo general:** llegar preparado a la propuesta del proyecto con la Secretaría de Administración y Finanzas de la CDMX (colaboración con el BID), con 4 workflows funcionando y documentados en 6 semanas (13 de octubre al 22 de noviembre).

**Qué hice**
- Armé el plan de preparación de 6 semanas.
- Creé este repositorio con su estructura, `docker-compose.yml` (n8n + PostgreSQL + Ollama opcional) y README.
- [ ] Cuenta en la consola de Claude con crédito y límite de gasto.
- [ ] Llave gratuita de Google AI Studio.
- [ ] Repo clonado y abierto en Cursor.

**Qué aprendí**
- Las suscripciones de chat (Claude Pro, Gemini) no incluyen acceso a la API; la API se paga por consumo.
- n8n Community Edition autoalojado es gratis y sin límite de ejecuciones; en gobierno importa porque los datos se quedan en infraestructura propia.

**Qué sigue (martes 13)**
- Levantar n8n con `docker compose up -d`.
- Primera mitad del curso Beginner de n8n.
- Primer workflow: formulario → Claude clasifica → fila en hoja de cálculo.

**Horas:** 1

---

## Plan de 6 semanas (resumen)

| Semana | Fechas | Enfoque | Entregable |
| --- | --- | --- | --- |
| 1 | 13–18 oct | Fundamentos: APIs, JSON, webhooks, n8n | Proyecto 1 básico |
| 2 | 20–25 oct | n8n a fondo; comparativa con Zapier y Make | Proyecto 1 completo + comparativa |
| 3 | 27 oct–1 nov | Python + API para documentos | Proyecto 2 |
| 4 | 3–8 nov | Datos abiertos y reportes programados | Proyecto 3 |
| 5 | 10–15 nov | RAG, agentes, IA local | Proyecto 4 |
| 6 | 17–22 nov | Portafolio y demo | Demo de 15 min + propuesta de casos |

Ritmo semanal: martes y jueves estudio (2 h), viernes construcción (3 h), sábado bloque largo (4 h), domingo documentar y planear (2–3 h).
