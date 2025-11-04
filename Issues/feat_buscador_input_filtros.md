# [Feat]: Buscador — Input y filtros

Descripción:
- Campo(s) y controles para realizar búsquedas de proveedores (texto, filtros por categoría/estado/rubro, fecha/fechas si aplica).

Epic padre
- [#Migración - Búsqueda de Proveedores] — Migración Frontend - Búsqueda de Proveedores

Archivos origen
- FormBusquedaProveedores.cpp, FormBusquedaProveedores.h, FormBusquedaProveedores.dfm (indicar líneas relevantes cuando se creen los issues de US)

Comportamientos clave (alto nivel)
- Búsqueda por texto libre (nombre, razón social, RUT/CIF).
- Filtros desplegables (rubro, estado, localidad) aplicables combinados.
- Autocompletado o sugerencias mientras se escribe.

Archivos a crear (sugeridos)
- ProviderSearchInput.tsx, ProviderFilters.tsx, providerSearch.module.css (o Tailwind).

Integración
- Endpoint a consumir (placeholder, confirmar con Backend):
  - GET /api/proveedores/search?query=&rubro=&estado=&page=&size=&sort=

Criterios de aceptación (alto nivel)
- Inputs permiten construir consultas equivalentes a las del legacy.
- Buen rendimiento (debounce, no llamadas innecesarias).
- Accesibilidad básica (labels, roles).

Definition of Done mínimo
- [ ] PR + tests unitarios/componente
- [ ] Mapa de trazabilidad (.cpp → nuevo código)