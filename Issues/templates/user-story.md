# [US]: <Título de la historia de usuario>

## Como/ Quiero / Para
_Declaración corta y orientada al usuario que define rol, acción y beneficio._
_Ejemplo: "Como administrativo, quiero que el campo 'Total' se calcule automáticamente al cambiar cantidad o precio para reducir errores manuales y agilizar la entrada de facturas"._

## Archivos origen
_Referencias concretas (archivo y líneas) del código legacy que motivan la historia._
- [archivo.cpp] (líneas), [archivo.h], [archivo.dfm]

## Entradas / Salidas de ejemplo
_Ejemplos de input y output esperados (datos, formatos, reglas de rounding)._
- Input: {...}
- Output esperado: {...} (reglas de rounding, tipos)

## Criterios de aceptación (Given / When / Then)
_Criterios verificables y concisos que definen el comportamiento esperado._
_Ejemplo:_
 - _Given un usuario en la página de catálogo con productos en varias categorías  
    When el usuario selecciona la categoría "Electrónica"  
    Then la lista muestra solo productos de la categoría "Electrónica"_
- Given: ..., When: ..., Then: ...
- Given: ..., When: ..., Then: ...
- Given: ..., When: ..., Then: ...

## Pruebas mínimas
_Lista de tests requeridos (unitarios, tests de componente y opcional e2e)._
- Tests unitarios (función crítica) — 3–4 casos
- Test de componente (RTL)
- Opcional: e2e (Cypress/Playwright)

## Definition of Done
_Checklist final que debe cumplirse para cerrar la historia (código TSX/TS, tests verdes, changelog con trazabilidad)._
- [ ] Código en React+TS
- [ ] Tests verdes y PR revisado
- [ ] Nota en changelog indicando qué líneas del .cpp se reimplementaron
