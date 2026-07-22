# DEMO-GOB Insomnia

Repositorio para los endpoints del backend DEMO-GOB/SISCAT.

## Uso en Insomnia

1. Crear proyecto con `Git Sync`.
2. Seleccionar el repo `Aaronchelo18/DEMO-GOB-INSOMNIA`.
3. Seleccionar la rama `main`.
4. Presionar `Scan for files`.
5. Elegir `my_collection.yaml` para importar los requests listos.

`openapi.yaml` queda como especificacion tecnica del API.

## Requests incluidos

- `GET /api/health`
- `GET /api/session`
- `GET /api/catalog`
- `GET /api/services`
- `GET /api/services/medicina/groups/infraestructura/items`
- `GET /api/services/enfermeria/groups/infraestructura/items`
- `GET /api/items/topico-lavamanos`
- `GET /api/captures`
- `POST /api/captures`

## Backend local

```text
http://127.0.0.1:8081
```

El backend puede levantarse desde `C:\DEMO-GOB_BACKEND` con:

```powershell
docker compose up -d --build
```
