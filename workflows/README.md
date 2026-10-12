# Workflows

Exportaciones JSON de n8n. Un subfolder por proyecto (por ejemplo `01-clasificador-solicitudes/`).

## Exportar desde n8n

Desde la carpeta raíz del repo, con n8n corriendo:

```bash
docker compose exec n8n n8n export:workflow --all --separate --pretty --output=/home/node/workflows/
```

Los archivos aparecen aquí mismo, porque esta carpeta está montada dentro del contenedor.

## Importar a n8n

```bash
docker compose exec n8n n8n import:workflow --separate --input=/home/node/workflows/
```

Antes de hacer commit, revisa que el JSON no contenga llaves ni datos personales. Las credenciales de n8n no se exportan dentro del workflow, pero los valores escritos directamente en un nodo sí.
