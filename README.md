# Palace-AutoPart
## 🚗 AutoParts Inventory System

Sistema de gestión de inventario para empresa de repuestos vehiculares
(Carros y Camionetas)

Stack Tecnológico:
- Frontend: React (JS)
- Backend: Django + Django REST Framework
- Base de Datos: PostgreSQL

---

## 🎯 Objetivo del Proyecto

Construir un sistema profesional de inventario que permita:

- Gestionar productos (repuestos)
- Controlar stock
- Registrar movimientos de entrada y salida
- Administrar proveedores
- Manejar usuarios con roles
- Optimizar consultas y rendimiento (enfoque DBA)

Este proyecto será desarrollado con enfoque profesional, no académico.

---

## 📦 Alcance del MVP (Fase 1 - Backend)

Primera fase enfocada únicamente en Backend + Base de Datos.

Debe incluir:

- Configuración de proyecto Django
- Conexión a PostgreSQL
- Modelos correctamente normalizados
- Migraciones
- CRUD vía API REST
- Autenticación básica
- Pruebas con Postman

NO incluye frontend en esta fase.

---

## 🧱 Modelo Inicial de Datos

### Brand
- id
- name

### Category
- id
- name

### VehicleType
- id
- name (Carro, Camioneta)

### Supplier
- id
- name
- contact_info

### Product
- id
- name
- sku (único)
- brand (FK)
- category (FK)
- vehicle_type (FK)
- price
- current_stock
- created_at

### StockMovement
- id
- product (FK)
- quantity
- movement_type (IN / OUT)
- created_at
- user (FK)

---

## ⚙️ Reglas de Negocio

- El stock no puede ser negativo.
- El SKU debe ser único.
- Todo movimiento debe estar asociado a un usuario.
- Las entradas aumentan stock.
- Las salidas disminuyen stock.

---

## 🧠 Objetivo Técnico Personal

Este proyecto busca:

- Dejar de depender de tutoriales.
- Pensar antes de codificar.
- Diseñar modelos sin copiar ejemplos.
- Implementar buenas prácticas.
- Documentar decisiones técnicas.

---

## 🔥 Reglas de Desarrollo

1. Intentar resolver problemas mínimo 45 minutos antes de buscar ayuda.
2. No copiar código directamente de IA.
3. Si se consulta solución, reescribir desde cero.
4. Subir avances constantes al repositorio.
5. Documentar errores y soluciones.

---

## 📅 Plan de Trabajo Inicial

Semana 1:
- Configuración del entorno
- Proyecto Django creado
- Conexión PostgreSQL funcionando
- Modelos definidos
- Migraciones ejecutadas

Semana 2:
- Serializers
- ViewSets
- Rutas
- CRUD funcional
- Pruebas en Postman

---

## 🧪 Futuras Fases

- Autenticación JWT
- Permisos por roles
- Optimización de consultas
- Índices y análisis de rendimiento
- Simulación de carga
- Frontend con React

---

## 📌 Estado del Proyecto

🟡 En desarrollo
