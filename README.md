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
- `DELETE /api/captures/{id}`
- `GET /api/uploads/{archivo}`
- `DELETE /api/uploads/{archivo}`

## Captures

- `GET /api/captures`: lista los informes guardados. Si la data esta limpia devuelve `captures: []`.
- `POST /api/captures`: guarda un informe. Puede recibir JSON sin archivo o `multipart/form-data` con fotos/PDF.
- `DELETE /api/captures/{id}`: elimina un informe completo usando el `id`, por ejemplo `cap_121f980b2d532cdb`.
- `GET /api/uploads/{archivo}`: previsualiza un archivo guardado usando el `stored_name`.
- `DELETE /api/uploads/{archivo}`: elimina un archivo guardado usando el `stored_name`.

## Backend local

```text
http://127.0.0.1:8081
```

El backend puede levantarse desde `C:\DEMO-GOB_BACKEND` con:

```powershell
docker compose up -d --build
```
