---
{"dg-publish":true,"dg-path":"🎮 Mecánicas y Sistemas/Core/Sistema de Mapeo.md","permalink":"/mecanicas-y-sistemas/core/sistema-de-mapeo/","dgPassFrontmatter":true}
---

Este es el sistema principal del juego. Es el núcleo del juego y todas las demás mecánicas tienen relación directa con esto. En cartographer's quest, tu tarea es crear mapas de las regiones que exploras para conocer sus secretos y mejorar su [[Documentation/Mécanicas y Sistemas/Estabilidad\|Estabilidad]]

# Mecánica Central del Mapeo

## Mapeo Automático Temporal
A medida que el jugador explora, el juego dibuja automáticamente un mapa que representa su recorrido y observaciones. Este mapa temporal tiene las siguientes características:

### Duración y Deterioro
- **Vida Limitada**: La información del mapa temporal se deteriora gradualmente con el tiempo
- **Deterioro Progresivo**: Las áreas más antiguas se desvanecen primero, siguiendo un orden cronológico
- **Factores de Deterioro**:
  - **Clima**: Condiciones adversas aceleran el desvanecimiento
  - **Hora del día**: Ciertos momentos del día afectan la retención de información
  - **Debuffs del jugador**: Estados negativos reducen la capacidad de retener información cartográfica
  - **Mejoras**: Herramientas y habilidades pueden ralentizar el deterioro

### Preservación en Campamentos
- **Registro Permanente**: En los [[Campamentos\|Campamentos]] el jugador puede "registrar" su mapa temporal
- **Proceso Instantáneo**: Presionar la acción de "registrar mapa" preserva instantáneamente la información actual
- **Sin Límites**: No hay restricciones en la cantidad de veces que se puede guardar
- **Información Permanente**: Una vez registrada, la información cartográfica no se deteriora

## Modos de Exploración

### Exploración Rápida
**Características**:
- **Cobertura Limitada**: Registra un área muy pequeña del recorrido
- **Alta Imprecisión**: Múltiples factores afectan la calidad del mapeo
- **Velocidad**: Permite avanzar rápidamente por el territorio

**Factores de Imprecisión**:
- **Climáticos**: Lluvia, niebla, viento reducen la precisión
- **Temporales**: Mapear de noche o en condiciones de poca luz
- **Estado del Jugador**: Fatiga, heridas, o debuffs negativos
- **Herramientas**: Equipamiento inadecuado para el terreno
- **Terreno**: Algunos tipos de terreno son inherentemente más difíciles de mapear

**Errores Típicos**:
- Desplazamientos en la posición de elementos
- Formas geográficas incorrectas o simplificadas
- Elementos importantes omitidos
- Escalas incorrectas

### Impresión Profunda
**Características**:
- **Área Circular**: Define un radio específico para exploración exhaustiva
- **Alta Precisión**: Registra la zona sin errores significativos
- **Tiempo Intensivo**: Requiere dedicación temporal considerable

**Variables del Sistema**:
- **Radio Variable**: Depende de las herramientas cartográficas disponibles
- **Tiempo de Completado**: Varía según:
  - Habilidad cartográfica del jugador
  - Calidad de las herramientas
  - Complejidad del terreno
  - Condiciones ambientales

**Proceso**:
1. El jugador selecciona el centro del área a mapear
2. Se establece un radio basado en herramientas
3. Debe explorar exhaustivamente toda el área del círculo
4. El sistema verifica la completitud antes de finalizar

# Interconexión con Otros Sistemas

## Relación con [[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de Conocimiento\|Sistema de Conocimiento]]
- **Exploración como Catalizador**: Aunque no hay relación directa con el mapeo, la exploración alimenta el sistema de conocimiento
- **Descubrimientos**: Elementos encontrados durante el mapeo pueden generar conocimiento

## Impacto en Expediciones
- **Precisión Crítica**: Los errores de mapeo afectan directamente el éxito de las [[Documentation/🎮 Mecánicas y Sistemas/Expediciones/Sistema de Equipos Expediciones\|expediciones]]
- **Planificación**: Mapas imprecisos pueden llevar a rutas peligrosas o ineficientes
- **Recursos**: Errores cartográficos pueden resultar en pérdida de recursos y tiempo

## Visualización del [[Documentation/🌍 Mundo/Conceptos/El Desvanecimiento\|El Desvanecimiento]]
- **Representación Visual**: El Desvanecimiento se refleja directamente en el mapa
- **Indicadores Cartográficos**: Áreas afectadas muestran cambios visuales específicos
- **Monitoreo**: El mapa sirve como herramienta de seguimiento del fenómeno

# Herramientas y Progresión

## Evolución del Equipamiento
Las herramientas cartográficas evolucionan a lo largo del juego, afectando múltiples aspectos:

### Factores Mejorados por Herramientas
- **Duración del Mapa Temporal**: Herramientas avanzadas mantienen la información por más tiempo
- **Precisión de Exploración Rápida**: Reducen los errores y aumentan el área cubierta
- **Radio de Impresión Profunda**: Permiten cubrir áreas más extensas
- **Resistencia al Deterioro**: Mejoran la resistencia a factores ambientales

### Especialización por Terreno
**Herramientas Específicas Requeridas**:
- **Cuevas y Subterráneos**: Equipamiento especial para navegación sin referencias celestes
- **Terrenos Acuáticos**: Herramientas para mapeo de costas y áreas inundables
- **Montañas**: Instrumentos para medición de altitudes y pendientes pronunciadas
- **Bosques Densos**: Equipamiento para navegación en áreas con visibilidad limitada
- **Terrenos Mágicos**: Herramientas especializadas para áreas con anomalías mágicas

## Desafíos Específicos por Entorno
Cada tipo de terreno presenta desafíos únicos que requieren adaptación de técnicas y herramientas.

# Características Visuales y de Experiencia

### Clima y Tiempo
Dependiendo de las condiciones, la visualización y la precisión del mapeo se verá afectada.

---
### Herramientas de anotación personalizable
Los jugadores pueden crear sus propias simbologías o usar símbolos tradicionales de cartografía.

---
### Estética de dibujo a mano
El mapa tendrá una estética de mapa de tela y con trazos estilizados

---
### Descubrimiento Orgánico
El juego NUNCA mostrará indicadores por UI. El jugador decide que observar y marcar en su mapa.

---
### Mapa en blanco
El mapa comienza estando completamente vacío y se va llenando a medida que exploras las zonas.

---
### Mapeo de cuevas e interiores
Se requieren técnicas especiales para mapear entornos interiores.

---
### Mapeo interactivo
Mini-juegos para la precisión del mapeo para puntos de interés importantes.

---
### Proceso de refinamiento del mapa
El mapa irá evolucionando de notas básicas a un producto final detallado.

---
### Progresión de las Herramientas de Mapeo
A medida que el jugador avanza irá desbloqueando herramientas más complejas que le permitirán mejorar su precisión.