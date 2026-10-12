# AI Automation Lab

Laboratorio personal de **automatización de procesos con inteligencia artificial** aplicado a la administración pública y las finanzas públicas.

Aquí documento lo que estudio, construyo y pruebo: workflows en n8n, integraciones con APIs de modelos de lenguaje (Claude, Gemini, modelos locales) y casos de uso pensados para una secretaría de finanzas.

> **Estado:** en construcción (octubre–noviembre de 2026). Cada semana se agrega un entregable funcional.

---

## Proyectos

| # | Proyecto | Qué resuelve | Estado |
| --- | --- | --- | --- |
| 1 | [Clasificador de solicitudes](projects/01-clasificador-solicitudes/) | Ordena y reparte solicitudes que llegan por correo o formulario | Pendiente |
| 2 | [Extractor de documentos](projects/02-extractor-documentos/) | Convierte facturas y oficios en datos estructurados | Pendiente |
| 3 | [Reporte de finanzas públicas](projects/03-reporte-finanzas-publicas/) | Genera reportes periódicos a partir de datos abiertos | Pendiente |
| 4 | [Agente de consulta normativa](projects/04-agente-normativa/) | Responde dudas sobre normativa citando la fuente | Pendiente |

## Principios de trabajo

- **Solo datos públicos o sintéticos.** Ningún dato real de personas o de instituciones se sube a este repositorio ni a herramientas externas.
- **Supervisión humana.** Toda decisión que afecte a una persona pasa por revisión humana.
- **Opciones adoptables por gobierno.** Prioridad a herramientas de código abierto y autoalojadas (los datos se quedan en infraestructura propia), con costos predecibles.
- **Transparencia.** Cada proyecto documenta su flujo, su costo estimado, sus riesgos y sus límites.

## Stack

- **Orquestación:** [n8n](https://n8n.io/) Community Edition, autoalojado con Docker.
- **Modelos:** API de Claude, API de Gemini y modelos locales con Ollama.
- **Código:** Python y JavaScript.
- **Base de datos:** PostgreSQL.

## Cómo correrlo

Requisitos: [Docker Desktop](https://www.docker.com/products/docker-desktop/) y Git.

```bash
git clone https://github.com/JoseShota/ai-automation-lab.git
cd ai-automation-lab
cp .env.example .env      # edita los valores (ver comentarios en el archivo)
docker compose up -d      # n8n queda en http://localhost:5678
```

Para usar modelos locales: `docker compose --profile local-ai up -d`.

## Estructura

```text
notes/       Apuntes de estudio y bitácora
workflows/   Workflows de n8n exportados (JSON)
projects/    Un folder por proyecto: documentación, diagrama, código y demo
data/        Solo datos públicos o sintéticos
docs/        Página de portafolio
```

---

## English summary

Personal lab for **AI-powered process automation** in public administration and public finance. It contains n8n workflows, LLM API integrations (Claude, Gemini, local models via Ollama) and four portfolio projects: a request classifier, a document extractor, an automated public-finance report and a regulation Q&A agent. Only public or synthetic data is used. Code, comments and commits are in English; project documentation is in Spanish.

## Autor

José Shōta Bustamante · [github.com/JoseShota](https://github.com/JoseShota)
