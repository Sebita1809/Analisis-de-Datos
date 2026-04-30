# Informe de Análisis — Transferencias de Automotores (Enero 2025)

**Parcial N°1 — Análisis de Datos COM3**  
**Integrantes:** Pablo Vivas, Lisandro Romero, Tobias Rivas, Morgui Mateo, Diaz Manuel, Diaz Sebastian  
**Dataset:** `tranferencias_autos.csv`  
**Registros analizados:** 162.837 (luego de eliminar 338 duplicados y 6.930 outliers)

---

## 1. Tipo de Automotor Más Transferido

Durante la limpieza se unificaron variantes de nomenclatura inconsistentes: `SEDAN 5 PTAS`, `SEDAN 4 PTAS`, `SEDAN 3 PTAS`, `RURAL 5 PTAS`, `RURAL 4 PTAS` y `RURAL 3 PTAS` fueron consolidadas con sus equivalentes de nombre completo.

| Posición | Tipo | Transferencias |
|----------|------|---------------|
| 1° | SEDAN 5 PUERTAS | 55.802 |
| 2° | SEDAN 4 PUERTAS | 34.538 |
| 3° | PICK-UP | 17.398 |
| 4° | SEDAN 3 PUERTAS | 13.305 |
| 5° | RURAL 5 PUERTAS | 12.535 |

**El tipo de automotor más transferido es el SEDAN 5 PUERTAS**, con 55.802 transferencias, representando el **34,3%** del total del dataset. El dominio de los sedán de cinco puertas es contundente: más que duplica al segundo tipo más transferido.

---

## 2. Marca con Mayor Cantidad de Transferencias

| Posición | Marca | Transferencias |
|----------|-------|---------------|
| 1° | VOLKSWAGEN | 30.242 |
| 2° | FORD | 21.556 |
| 3° | CHEVROLET | 19.250 |
| 4° | RENAULT | 18.778 |
| 5° | FIAT | 16.642 |

**VOLKSWAGEN es la marca con mayor cantidad de transferencias**, con 30.242 unidades, representando el **18,6%** del total. Cabe destacar que tras la eliminación de outliers, CHEVROLET superó a RENAULT en el tercer puesto respecto al análisis preliminar sin filtrar.

---

## 3. Provincia con Más Transferencias

| Posición | Provincia | Transferencias |
|----------|-----------|---------------|
| 1° | Buenos Aires | 61.317 |
| 2° | Córdoba | 18.760 |
| 3° | CABA | 14.815 |
| 4° | Santa Fe | 13.466 |
| 5° | Mendoza | 7.853 |

**Buenos Aires concentra la mayor cantidad de transferencias**, con 61.317 registros que representan el **37,7%** del total nacional. Junto con Córdoba, CABA y Santa Fe, estas cuatro provincias acumulan más del **66%** de todas las transferencias del país, evidenciando una fuerte concentración en la región centro y pampeana.

---

## 4. Marca Líder por Provincia

| Provincia | Marca Líder | Transferencias |
|-----------|-------------|---------------|
| Buenos Aires | VOLKSWAGEN | 12.262 |
| Córdoba | VOLKSWAGEN | 3.109 |
| CABA | VOLKSWAGEN | 2.328 |
| Santa Fe | VOLKSWAGEN | 2.146 |
| Mendoza | VOLKSWAGEN | 1.320 |
| Entre Ríos | VOLKSWAGEN | 1.368 |
| Neuquén | VOLKSWAGEN | 858 |
| Río Negro | VOLKSWAGEN | 622 |
| Tucumán | VOLKSWAGEN | 681 |
| Corrientes | VOLKSWAGEN | 661 |
| Chubut | **FORD** | 582 |
| Misiones | VOLKSWAGEN | 542 |
| Chaco | VOLKSWAGEN | 557 |
| La Pampa | VOLKSWAGEN | 538 |
| Salta | VOLKSWAGEN | 562 |
| San Luis | VOLKSWAGEN | 426 |
| San Juan | VOLKSWAGEN | 365 |
| Santa Cruz | **FORD** | 292 |
| Jujuy | VOLKSWAGEN | 214 |
| Santiago del Estero | VOLKSWAGEN | 254 |
| Tierra del Fuego | VOLKSWAGEN | 134 |
| Formosa | **TOYOTA** | 269 |
| Catamarca | VOLKSWAGEN | 154 |
| La Rioja | VOLKSWAGEN | 175 |

**VOLKSWAGEN lidera en 21 de las 24 provincias**. Las únicas excepciones son Chubut y Santa Cruz, donde FORD toma la delantera, y Formosa, donde TOYOTA es la marca con más transferencias.

---

## 5. Automotor Líder por Provincia

| Provincia | Tipo Líder | Transferencias |
|-----------|------------|---------------|
| Buenos Aires | SEDAN 5 PUERTAS | 21.833 |
| Córdoba | SEDAN 5 PUERTAS | 6.506 |
| CABA | SEDAN 5 PUERTAS | 5.842 |
| Santa Fe | SEDAN 5 PUERTAS | 4.568 |
| Mendoza | SEDAN 5 PUERTAS | 2.396 |
| Entre Ríos | SEDAN 5 PUERTAS | 2.024 |
| Neuquén | SEDAN 5 PUERTAS | 1.377 |
| Tucumán | SEDAN 5 PUERTAS | 1.196 |
| Río Negro | SEDAN 5 PUERTAS | 1.102 |
| Corrientes | SEDAN 5 PUERTAS | 910 |
| Chubut | SEDAN 5 PUERTAS | 936 |
| Chaco | SEDAN 5 PUERTAS | 810 |
| Misiones | SEDAN 5 PUERTAS | 880 |
| La Pampa | SEDAN 5 PUERTAS | 795 |
| Salta | SEDAN 5 PUERTAS | 796 |
| San Luis | SEDAN 5 PUERTAS | 678 |
| San Juan | SEDAN 5 PUERTAS | 685 |
| Santa Cruz | SEDAN 5 PUERTAS | 471 |
| Jujuy | SEDAN 5 PUERTAS | 416 |
| Santiago del Estero | SEDAN 5 PUERTAS | 349 |
| Tierra del Fuego | SEDAN 5 PUERTAS | 389 |
| Formosa | SEDAN 5 PUERTAS | 271 |
| Catamarca | SEDAN 5 PUERTAS | 275 |
| La Rioja | SEDAN 5 PUERTAS | 297 |

**El SEDAN 5 PUERTAS es el tipo de automotor líder en las 24 provincias**, sin excepción.

---

## 6. Diferencia entre Persona Física y Persona Jurídica

| Tipo de Titular | Cantidad | Porcentaje |
|-----------------|----------|------------|
| Persona Física | 153.707 | 94,4% |
| Persona Jurídica | 9.130 | 5,6% |
| **Total** | **162.837** | **100%** |

**La diferencia absoluta entre personas físicas y jurídicas es de 144.577 transferencias.**

El mercado de transferencias está absolutamente dominado por **personas físicas**, que representan el 94,4% de las operaciones. Las personas jurídicas participan de manera marginal con apenas el 5,6%, evidenciando que el mercado de usados en Argentina es eminentemente particular.

---

## 7. Feature Engineering — Nuevas Variables Creadas

### Variable: `automotor_antiguedad`
Representa la cantidad de años del vehículo al momento de la transferencia, calculada como `2025 - automotor_anio_modelo`.

| Estadístico | Valor |
|-------------|-------|
| Registros con año declarado | 162.045 |
| Antigüedad promedio | 13,1 años |
| Desvío estándar | 7,3 años |
| Mínimo | 0 años |
| Mediana | 12 años |
| Máximo | 33 años |

### Variable: `automotor_categoria_antiguedad`
Categorización de la antigüedad en tres rangos:

| Categoría | Cantidad | Porcentaje |
|-----------|----------|------------|
| Usado (6-15 años) | 92.537 | 56,8% |
| Antiguo (+15 años) | 48.767 | 29,9% |
| Casi nuevo (0-5 años) | 20.741 | 12,7% |
| No especificado | 792 | 0,5% |

**El mercado de transferencias está dominado por vehículos usados de entre 6 y 15 años de antigüedad**, que representan más de la mitad de todas las operaciones (56,8%). Los vehículos casi nuevos (hasta 5 años) son una minoría con apenas el 12,7%, lo que refleja que el mercado de usados en Argentina opera principalmente con autos de mediana antigüedad.

---

## Proceso de Limpieza y Calidad de Datos

| Etapa | Registros |
|-------|-----------|
| Dataset original | 170.105 |
| Tras eliminación de duplicados | 169.767 |
| Tras eliminación de outliers (IQR) | 162.837 |
| **Dataset final analizado** | **162.837** |

**Outliers eliminados por IQR:** 6.930 registros correspondientes a vehículos con año modelo anterior a 1992 o posterior a 2032 (límites: Q1=2007, Q3=2017, IQR=10).

---

## Conclusiones Generales

- El mercado de transferencias en Argentina (enero 2025) está fuertemente concentrado en la región pampeana, con **Buenos Aires** como provincia dominante (37,7% del total).
- **VOLKSWAGEN** lidera en 21 de las 24 provincias, con una presencia nacional sin rival.
- El **SEDAN 5 PUERTAS** es el tipo de vehículo de preferencia unánime en todo el país (34,3% del total), liderando en las 24 provincias sin excepción.
- El mercado es esencialmente **particular**: las personas físicas representan el 94,4% de las operaciones frente al 5,6% de personas jurídicas.
- En cuanto a la antigüedad, el mercado opera mayoritariamente con **vehículos usados de 6 a 15 años** (56,8%), siendo los autos casi nuevos una minoría del 12,7%.
