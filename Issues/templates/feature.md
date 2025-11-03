# [Feat]: <Título de la Feature>

## Descripción
_Descripción concisa del valor funcional que ofrece la feature_

## Epic padre
_Referencia a la épica que agrupa la feature (ID/título)._
- [#epic-id] — Título Epic

## Archivos origen
_Archivos .cpp/.h/.dfm relevantes (rutas o líneas si están disponibles) que orientan la migración_
- [archivo.cpp], [archivo.h], [archivo.dfm] (rutas/líneas relevantes)

## Comportamientos clave (alto nivel)
_2–4 flujos o casos de uso principales que la feature debe soportar (sin entrar en Given/When/Then)._

## Archivos a crear (sugeridos)
_Lista de componentes, hooks, servicios y stories que deberían generarse._
_- Ej.: InvoiceForm.tsx, useInvoice.ts, invoiceService.ts, Invoice.stories.tsx_

## Integración
_Endpoints y contratos backend que la feature consumirá (nombres y parámetros fundamentales)._
_- Ej.: POST /api/invoices_

## Criterios de aceptación (alto nivel)
_- Condiciones de integración y no funcionales (p. ej. coverage objetivo, accesibilidad)._

## Definition of Done mínimo
_Checklist de entrega (PR, tests, storybook, trazabilidad)._
- [ ] PR + tests unitarios/componente
- [ ] Storybook / demo
- [ ] Mapa de trazabilidad (.cpp → nuevo código)
