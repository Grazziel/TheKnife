# TheKnife - Gestión de Restaurante

Aplicación full-stack de gestión de restaurantes con distintos roles de usuario (jefe de cocina y camarero), desarrollada en equipo como proyecto del bootcamp Full-Stack de 4Geeks Academy.

## Stack técnico
- Backend en Flask (API REST)
- Frontend en React (hooks personalizados: `useGlobalReducer`, `useChef`, `useRestaurant`)
- Autenticación por token, guardado en `localStorage`

## Funcionalidades

**Rol jefe de cocina**
- Registro y login
- CRUD de restaurante
- CRUD de recetas e ingredientes
- CRUD de comandas/pedidos
- CRUD de cocineros, camareros, mesas y productos

**Rol camarero**
- Login
- Consulta de las recetas de su restaurante
- Creación de comandas
- Consulta de las comandas de su restaurante
- Actualización del estado de una comanda
- CRUD de las mesas de su restaurante

## Mi contribución (Graziele)

Desarrollé el flujo del rol **camarero** (rama `ft-23-flujo-camarero`), siguiendo el mismo patrón de arquitectura ya implementado para el rol de jefe de cocina:
- Servicio para consultar las recetas del restaurante a partir del token del camarero (decodificando el token para obtener el `restaurant_id`, en vez de pasarlo manualmente)
- Creación y consulta de comandas
- Actualización del estado de las comandas
- CRUD de mesas del restaurante

## Cómo correrlo localmente
```bash
pipenv install
pipenv run start
```
En otra terminal, para el frontend:
```bash
npm install
npm start
```

---
Proyecto en equipo desarrollado como parte del bootcamp Full-Stack de 4Geeks Academy.
