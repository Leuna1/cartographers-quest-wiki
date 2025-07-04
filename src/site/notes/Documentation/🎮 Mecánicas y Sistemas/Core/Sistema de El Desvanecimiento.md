---
{"dg-publish":true,"dg-path":"🎮 Mecánicas y Sistemas/Core/Sistema de El Desvanecimiento.md","permalink":"/mecanicas-y-sistemas/core/sistema-de-el-desvanecimiento/","dgPassFrontmatter":true}
---


[[Documentation/🌍 Mundo/Conceptos/El Desvanecimiento\|El Desvanecimiento]] es el desafío principal del juego. Una representación visual y mecánica de la desaparición del mundo de la realidad. Esta mecánica antagonista se opone directamente al [[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de Mapeo\|Sistema de Mapeo]], creando tensión constante entre exploración y preservación.

## Mecánica Base

### Independencia Regional
Cada región tiene su propio porcentaje de estabilidad (0%-100%) que decae independientemente. El desvanecimiento no se propaga entre regiones, pero la pérdida de regiones clave puede afectar las bonificaciones de red.

### Velocidad de Decadencia
La velocidad de pérdida de estabilidad es arbitraria y se define durante el balanceo del juego, considerando:
- Tamaño de la región
- Punto en la historia donde el jugador la encuentra
- Importancia narrativa
- Factores específicos de cada región

## Implementación Visual

#### 1er Estado: Alertas Tempranas (Estabilidad 40% - 69%)

1. Los colores se ven más opacos
2. El borde de los objetos titilan y parecen un poco transparentes
3. Partículas pequeñas de luz se alzan desde el suelo
4. El sonido se vuelve hueco y distante

#### 2do Estado: Desvanecimiento Activo (Estabilidad 20% - 39%)

1. Los objetos y el terreno se vuelve más semitransparentes
2. El borde de la tierra se ve erosionada con pedazos separados
3. Ondas visuales aparecen en el terreno
4. En el mapa estas áreas aparecen distorsionadas o con partes faltantes

#### 3er Estado: Casi Perdido (Estabilidad 1% - 19%)

1. El piso se rompe en fragmentos flotantes
2. Estática estilo TV aparece en áreas gravemente afectadas
3. Partes del mundo son reemplazadas por espacios vacíos
4. El movimiento se vuelve inestable

#### 4to Estado: Desvanecimiento Total (Estabilidad 0%)

1. Las zonas están completamente vacías
2. Los bordes del desvanecimiento tiene efectos visuales dramáticos
3. Los jugadores no pueden entrar áreas completamente desvanecidas (hasta obtener habilidades especiales más tarde en la historia)
4. Las áreas desvanecidas tienen ecos ligeros de lo que existía ahí antes
5. SOLO las áreas generadas por código se pueden desvanecer
6. Las áreas importantes de la historia solo pueden bajar hasta 1%

## Sistema de Estabilidad y Anclajes

### Estabilidad Mínima
Los [[Documentation/🌍 Mundo/Anclajes de Estabilidad\|Anclajes de Estabilidad]] establecen un nivel mínimo de estabilidad para cada región:
- **Sin anclajes**: Estabilidad mínima = 0%
- **Con anclajes**: Estabilidad mínima = suma de protección de todos los anclajes

**Ejemplo**: Una región con un anclaje que aporta 2% de protección tendrá una estabilidad mínima del 2%, nunca podrá bajar de ese nivel.

### Tipos de Anclajes
- **Anclajes de Protección**: Aumentan el mínimo de estabilidad de la región
- **Anclajes de Ralentización**: Reducen la velocidad de decadencia sin aumentar el mínimo
- **Anclajes de Área**: Protegen zonas específicas dentro de la región
- **Anclajes Mixtos**: Combinan múltiples efectos
- Más anclajes TBD

### Descubrimiento de Anclajes
Al descubrir un anclaje:
1. Se obtiene un aumento inmediato de estabilidad
2. Se activa la protección/efecto del anclaje
3. Este aumento inicial puede seguir decayendo con el tiempo, pero nunca por debajo del mínimo establecido

## Recuperación de Estabilidad

### Acciones que Aumentan Estabilidad
1. **Exploración básica**: Aumento bajo de estabilidad
2. **Mapeo detallado**: Aumento medio de estabilidad
3. **Expediciones**: Contribución significativa a la estabilidad
4. **Documentar puntos de anclaje**: Gran aumento de estabilidad
5. **Interacción con otros sistemas**: Casi toda actividad del jugador afecta positivamente la estabilidad

### Dificultad de Recuperación
- La recuperación no se vuelve más difícil en niveles críticos
- El proceso es consistente independientemente del nivel actual
- Los anclajes facilitan la recuperación al establecer un "piso" de seguridad

## Interacción con Otros Sistemas

### Sistema de Campamentos
- **Campamentos Rápidos**: Vulnerables al desvanecimiento, se pierden si la región llega a 0%
- **Bases (Campamentos Grandes)**: Solo se pueden construir alrededor de ciertos puntos de anclaje para garantizar su permanencia

### Sistema de Conocimiento
- **El conocimiento NUNCA se pierde**, incluso si la región se desvanece completamente
- Los mapas y datos recolectados permanecen disponibles
- Esta información será crucial para la eventual recuperación de regiones perdidas

### Progresión Narrativa
- Más adelante en la historia, el jugador obtendrá habilidades para viajar por el desvanecimiento
- Las regiones importantes para la historia nunca pueden desvanecerse completamente (mínimo 1%)

## Sistema de Priorización de Regiones

### Recursos Únicos por Región
Cada región contiene recursos específicos que se vuelven inaccesibles si se desvanece:
- **Minerales raros**: Necesarios para equipamiento avanzado
- **Plantas medicinales**: Requeridas para pociones y curaciones especiales
- **Materiales de construcción**: Únicos para ciertas mejoras de campamento
- **Artefactos culturales**: Elementos narrativos y de colección

### Bonificaciones de Red
Las regiones estables y conectadas proporcionan bonificaciones sinérgicas:
- **Velocidad de exploración aumentada** en regiones conectadas
- **Eficiencia de recursos mejorada** en redes estables
- **Bonificaciones de conocimiento** por mantener rutas de información abiertas
- **Efectos acumulativos** que crecen con el tamaño de la red estable

### Eventos Temporales
Las regiones estables pueden albergar eventos especiales:
- **Comerciantes nómadas** que solo visitan áreas seguras
- **Eventos de investigación** que requieren estabilidad mínima
- **Encuentros narrativos únicos** que se pierden si la región se desvanece
- **Oportunidades de expedición especiales** disponibles temporalmente

## Estrategias de Gestión

### Decisiones Tácticas
El jugador debe constantemente evaluar:
- **Costo de oportunidad**: ¿Vale la pena estabilizar esta región ahora?
- **Importancia estratégica**: ¿Esta región conecta otras áreas importantes?
- **Recursos disponibles**: ¿Tengo los recursos necesarios para múltiples regiones?
- **Urgencia temporal**: ¿Qué regiones están en peligro inmediato?

### Recuperación vs Prevención
- **Prevención**: Mantener estabilidad es más eficiente que recuperar regiones perdidas
- **Recuperación**: Las regiones desvanecidas pueden recuperarse, pero requiere más esfuerzo
- **Priorización**: Algunas regiones opcionales pueden sacrificarse temporalmente por otras más críticas

## Balanceo y Tensión

### Presión Constante
El desvanecimiento crea una presión constante que:
- Impide que el jugador se estanque en una sola área
- Fuerza decisiones difíciles sobre priorización de recursos
- Mantiene la urgencia narrativa del mundo que desaparece
- Recompensa la planificación estratégica a largo plazo

### Alivio Progresivo
A medida que el jugador progresa:
- Los anclajes proporcionan mayor seguridad
- Las habilidades de viaje por el desvanecimiento abren nuevas posibilidades
- Las bonificaciones de red hacen más eficiente la gestión
- El cono-cimiento acumulado facilita la toma de decisiones


