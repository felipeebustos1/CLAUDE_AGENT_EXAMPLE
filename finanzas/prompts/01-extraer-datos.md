# Paso 1: Extraer datos del seguimiento interno

Vas a cruzar la información de `context/` con las notas de `inputs/` para extraer los datos de la reunión interna de seguimiento de clientes. Esta reunión es entre el equipo, no con el cliente.

## Fuentes

- `context/`: material de referencia. Incluye la tabla de facturación, los contratos activos, las propuestas en curso, las fichas de clientes nuevos, la información de marketing y de eventos o ferias, y el archivo de participantes.
- `context/participantes.md`: lista de involucrados con su rol y las áreas en las que participan. Tiene este formato:

  | Persona | Rol | Facturación | Contratos activos | Plan de acción nuevos clientes | Marketing | Eventos y ferias |
  |---|---|---|---|---|---|---|
  | (nombre) | (rol) | sí / no | sí / no | sí / no | sí / no | sí / no |

- `inputs/`: notas libres de la reunión interna. Pueden ser desordenadas, incompletas o con abreviaturas.

## Instrucciones

1. Lee `context/participantes.md` primero. Ese archivo define a quién corresponde cada área.
2. Lee el resto de `context/` y `inputs/`.
3. Extrae únicamente lo que aparezca en las fuentes. No inventes cifras, fechas, clientes ni compromisos.
4. Organiza la información en cinco áreas generales:
   - **Facturación**
   - **Contratos activos**
   - **Plan de acción nuevos clientes**
   - **Marketing**
   - **Eventos y ferias**
5. Para las tres primeras áreas, agrupa además la información por persona. Solo incluye a una persona en un área si `context/participantes.md` indica que participa en ella. Si las notas mencionan a alguien en un área en la que no participa, o un área sin responsable definido, márcalo como **discrepancia**.
6. Por cada cliente, registra cuando aparezca: nombre, cifra, estado, responsable y fecha.
7. Si falta un dato necesario, escribe `NO INDICADO` en lugar de suponerlo.
8. Si una cifra de las notas contradice `context/`, márcala como **discrepancia** y no decidas cuál es la correcta.

## Salida

Devuelve un bloque con esta estructura:

```
Fecha de la reunión:
Participantes presentes:

FACTURACIÓN
  Generales:
  Por persona:
    [Nombre]: (solo si participa en Facturación)

CONTRATOS ACTIVOS
  Generales:
  Por persona:
    [Nombre]: (solo si participa en Contratos activos)

PLAN DE ACCIÓN NUEVOS CLIENTES
  Generales:
  Por persona:
    [Nombre]: (solo si participa en Plan de acción nuevos clientes)

MARKETING
  Temas, responsables, fechas:

EVENTOS Y FERIAS
  Temas, responsables, fechas:

COMPROMISOS (acción | responsable | fecha):
DECISIONES TOMADAS:
DISCREPANCIAS DETECTADAS:
DATOS FALTANTES:
```

Cada cifra debe indicar de qué archivo sale, por ejemplo `(fuente: context/contratos.md)` o `(fuente: inputs/notas-seguimiento.txt)`.
