# [Epic]: Migración Búsqueda de Proveedores

Resumen
- Migrar la interfaz de búsqueda de proveedores desde C++ Builder (FormBusquedaProveedores) a React + TypeScript, consumiendo los endpoints del backend Spring Boot.

Contexto
- Módulo origen: Búsquedas — Proveedores
- Archivos: FormBusquedaProveedores.cpp, FormBusquedaProveedores.h, FormBusquedaProveedores.dfm

Objetivo / Criterios de éxito
- UI en React equivalente y usable por usuarios actuales.
- Lógica de filtrado/validación migrada y cubierta por tests.
- Integración con los endpoints del backend exitosa.

Alcance (Incluye / Excluye)
- Incluye: componente(es) de búsqueda, filtros, listado de resultados, paginación, detalle de proveedor, servicios/hooks para consumo de API, tests unitarios y de componente, Storybook.
- Excluye: cambios en backend (salvo acuerdos de contrato), migraciones de otros módulos no relacionados.

Entregables
- Features:
  - Buscador — Input y filtros
  - Resultados — Lista, paginación y orden
  - Detalle de proveedor (modal/page)
  - Integración API / Hook useProviderSearch
  - Tests, Storybook y accesibilidad

Dependencias / Riesgos
- Dependencias críticas: contratos de API con Backend Team (endpoints de búsqueda y detalle).
- Riesgo principal: ausencias de documentación completa del código legado (.cpp/.h/.dfm) que impidan reproducir reglas de filtrado; mitigación: solicitar snippets o ejemplos de datos.

Definition of Done mínimo
- [ ] Features enlazadas
- [ ] Validación de testing en el PR
- [ ] Documentación de migración (mapa .cpp → nuevos archivos) incluida en PR

## Perfiles de usuario:
- usuario administrativo del sistema