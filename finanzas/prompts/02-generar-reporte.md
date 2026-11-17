# Paso 2: Generar el reporte de seguimiento interno

Usa los datos extraídos en el paso 1 para redactar el reporte interno de seguimiento de clientes. Es un documento para el equipo, no para el cliente.

## Entrada

- El bloque de datos producido por `01-extraer-datos.md`.
- Si hace falta confirmar un detalle, consulta `context/` directamente.

## Instrucciones

1. Redacta en español, en tono profesional y directo.
2. Usa solo los datos del paso 1. Si un campo está como `NO INDICADO`, déjalo así o omite la fila. No lo completes.
3. En la sección por involucrado, muestra solo las áreas en las que esa persona participa, según `context/participantes.md`. No muestres áreas en las que no participa.
4. Incluye las discrepancias en su propia sección, para que el equipo las revise.
5. Cierra con los compromisos, con responsable y fecha cuando existan.

## Formato del reporte

```
# Reporte interno de seguimiento de clientes - [fecha]

## Resumen
(3 a 5 líneas con lo más importante del periodo)

## Generales

### 1. Facturación
(tabla: cliente | concepto | monto | estado | responsable | fuente)

### 2. Contratos activos
(tabla: cliente | contrato | vigencia | estado | responsable | fuente)

### 3. Plan de acción nuevos clientes
(tabla: cliente | etapa | próxima acción | responsable | fecha | fuente)

## Por involucrado
(una subsección por persona, con solo las áreas en las que participa)

### [Nombre] - [Rol]
- **Facturación:** ...
- **Contratos activos:** ...
- **Plan de acción nuevos clientes:** ...

## 4. Marketing
(temas, avances, responsables, fechas)

## 5. Eventos y ferias
(evento o feria | fecha | estado | responsable | fuente)

## 6. Compromisos y próximos pasos
(tabla: acción | responsable | fecha)

## 7. Discrepancias a revisar

## 8. Datos pendientes
```

Guarda el resultado como `finanzas/reporte-seguimiento-[fecha].md` si el usuario lo pide.
