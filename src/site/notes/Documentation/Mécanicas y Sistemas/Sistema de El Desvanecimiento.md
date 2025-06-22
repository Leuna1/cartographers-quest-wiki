---
{"dg-publish":true,"dg-path":"Mécanicas y Sistemas/Sistema de El Desvanecimiento.md","permalink":"/mecanicas-y-sistemas/sistema-de-el-desvanecimiento/","dgPassFrontmatter":true}
---


[[Documentation/Conceptos/El Desvanecimiento\|El Desvanecimiento]] es el desafío principal del juego. Una representación visual y mecánica de la desaparición del mundo de la realidad.

## Implementación visual

#### 1er Estado: Alertas tempranas (Estabilidad 40% - 69%)

1. Los colores se ven más opacos
    
2. El borde de los objetos titilan y parecen un poco transparentes
    
3. Partículas pequeñas de luz se alzan desde el suelo
    
4. El sonido se vuelve hueco y distante
    

#### 2do Estado: Desvanecimiento Activo (Estabilidad 20% - 39%)

1. Los objetos y el terreno se vuelve más semitransparentes
    
2. El borde de la tierra se ve erosionada con pedazos separados
    
3. Ondas visuales aparecen en el terreno
    
4. En el mapa estas áreas aparecen distorsionadas o con partes faltantes.
    

#### 3er Estado: Casi Perdido (Estabilidad 1% - 19%)

1. El piso se rompe en fragmentos flotantes
    
2. Estática estilo TV aparece en áreas gravemente afectadas
    
3. Partes del mundo son reemplazadas por espacios vacíos
    
4. El movimiento se vuelve inestable
    

#### 4to Estado: Desvanecimiento Total (Estabilidad 0%)

1. Las zonas están completamente vacías
    
2. Los bordes del desvanecimiento tiene efectos visuales dramáticos
    
3. Los  jugadores no pueden entrar áreas completamente desvanecidas
    
4. Las áreas desvanecidas tienen ecos ligeros de lo que existía ahí antes
    
5. SOLO las áreas generadas por código se pueden desvanecer
    
6. Las áreas importantes de la historia solo pueden bajar hasta 1%

## Implementaciones de Jugabilidad

#### Estabilidad Regional

1. Cada región tendrá un porcentaje de estabilidad (0%-100%)
    
2. Regiones sin mapear pierden un porcentaje fijo de estabilidad por día (Varía de acuerdo a la región)
    
3. Ciertos eventos pueden afectar la decadencia de la estabilidad
    
4. La exploración básica agrega un porcentaje bajo de estabilidad
    
5. El mapeo detallado agrega una estabilidad media
    
6. Documentar los puntos de anclaje aumenta la estabilidad mucho
    
7. La estabilidad siempre caerá hasta que se relacionen los anclajes


