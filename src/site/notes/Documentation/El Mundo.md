---
{"dg-publish":true,"dg-path":"El Mundo.md","permalink":"/el-mundo/","dgPassFrontmatter":true}
---

# Generación Hibrida
## Cambios Estacionales

El mundo cambia visualmente y funcionalmente de acuerdo a la temporada actual, afectando el reto al mapear.

A medida que se avanza en el juego el tiempo ira transcurriendo. El [[Documentation/Mécanicas y Sistemas/Paso del Tiempo\|pasar del tiempo]] traerá consigo diferentes estaciones (Invierno, verano, otoño y primavera). Esto causara que cada región sufra cambios importantes que pueden afectar diferentes sistemas del juego.

---
## Esquema Continental

Masas de tierra construidas a mano con biomas distintivos y puntos de interés claves.

Las áreas importantes del juego serán construidas a mano. Esto quiere decir que serán prediseñadas e iguales entre diferentes instancias del juego. 

El objetivo de esto es que estas zonas serán mas vivas y con mayor atención al detalle, con eventos pre-diseñados y con [[Puntos de Interés\|puntos de interés]] importantes para la narrativa.

---
## Estabilidad Variable

Cada región tiene su propia resistencia a [[Documentation/Conceptos/El Desvanecimiento\|El Desvanecimiento]]. Creando una priorización natural. Esto depende netamente de la [[Documentation/Mécanicas y Sistemas/Estabilidad\|Estabilidad]] de la región

---
## Plantillas Regionales

Tipos de regiones pre-diseñadas (Bosque antiguo, Archipiélagos volcánicos, etc.) con temas y desafíos consistentes.

---
## Puntos de anclajes Narrativos

[[Anclajes de Estabilidad\|Anclajes de Estabilidad]] localizados en zonas pre-diseñadas importantes para la historia puestos dentro de los algoritmos de generación.

---
## Relleno Procedural

Terrenos, caminos, puntos de interés y recursos generados por algoritmos.

Gran parte del terreno se llenara proceduralmente, haciendo que la experiencia de cada jugador sea distinta. Los desafíos se encontraran en diferentes lugares así como las zonas pre-diseñadas.

---
# Implementación

## Generación por capas
Se comienza con el esqueleto del mundo posicionando las zonas importantes y pre-diseñadas, después se le aplican capas de algoritmos que respetan las restricciones regionales

## Reglas de Bioma
Cada bioma tiene sus propias reglas de generación (Densidad de bosques, formación de elevaciones, etc.)

## Dificultad Gradual
Progresión gradual de dificultad al avanzar por las regiones, con elementos procedurales escalando acorde.

## Integración Narrativa
Las localizaciones importantes para la narrativa se mantienen consistentes, mientras que el camino entre ellas cambia de juego en juego.

## Mundo Dinámico
El entorno cambia de acuerdo a las estaciones y acciones del jugador.

## Visualización de El Desvanecimiento
Las regiones muestran indicios claros de la estabilidad del mapa de acuerdo al progreso del mapeo