# [US]: Buscar proveedores por texto básico

Como(usuario)
- Como usuario administrativo / operador de sistema

Quiero(acción)
- Quiero buscar proveedores por nombre, razón social o RUT/CIF desde el campo de búsqueda

Para(beneficio)
- Para encontrar rápidamente el proveedor que necesito sin usar el sistema legacy

Archivos origen
- FormBusquedaProveedores.cpp (sección de búsqueda por texto) — indicar líneas cuando se disponga

Entradas / Salidas de ejemplo
- Input: query="Distribuciones Norte"
- Output esperado: lista paginada de proveedores cuyo nombre contiene "Distribuciones Norte"

Criterios de aceptación (Given / When / Then)
- Given: el usuario está en la pantalla de búsqueda  
  When: ingresa "Distribuciones Norte" y presiona Enter 
  Then: se muestra la lista de proveedores que coinciden con el texto

Pruebas mínimas
- Tests unitarios para el mapeo de resultados
- Test de componente (RTL) que simula escribir y mostrar resultados

Definition of Done
- [ ] Código en React+TS
- [ ] Tests verdes y PR revisado
