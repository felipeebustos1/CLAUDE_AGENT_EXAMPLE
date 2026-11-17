# Paso 1: Extraer datos

Vas a cruzar la información de `context/` con las notas de `inputs/` para extraer los datos clave de la reunión.

## Fuentes

- `context/`: tabla de datos, propuesta, ficha del cliente, etc. Es la referencia de verdad sobre cifras, nombres y productos.
- `inputs/`: notas libres de la reunión. Pueden ser desordenadas, incompletas o con abreviaturas.

## Instrucciones

1. Lee todos los archivos de `context/` y `inputs/`.
2. Extrae únicamente lo que aparezca en las fuentes. No inventes cifras, fechas ni compromisos.
3. Cruza las notas con el contexto: si una cifra de la reunión contradice la tabla o la propuesta, márcala como **discrepancia**.
4. Si falta un dato necesario, escribe `NO INDICADO` en lugar de suponerlo.

## Salida

Devuelve un bloque con esta estructura:

```
Cliente:
Fecha de la reunión:
Participantes:
Temas tratados:
Cifras mencionadas (con fuente):
Compromisos y próximos pasos (responsable, fecha):
Decisiones tomadas:
Riesgos u objeciones:
Discrepancias detectadas:
Datos faltantes:
```

Cada cifra debe indicar de qué archivo sale, por ejemplo `(fuente: context/propuesta.md)` o `(fuente: inputs/notas-reunion.txt)`.
