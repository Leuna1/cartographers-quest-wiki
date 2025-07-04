---
{"dg-publish":true,"dg-path":"📖 Documentación Principal/El Mundo.md","permalink":"/documentacion-principal/el-mundo/","dgPassFrontmatter":true}
---


# El Mundo de Cartographer's Quest
*Guía de Diseño y Desarrollo*

## Resumen Ejecutivo

El mundo de Cartographer's Quest utiliza un sistema de **generación híbrida** que combina áreas pre-diseñadas narrativamente importantes con contenido procedural dinámico. El diseño está centrado en crear urgencia a través de [[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de El Desvanecimiento\|El Desvanecimiento]] y proporcionar una experiencia de exploración única en cada partida.

**Pilares de Diseño:**
- Urgencia temporal a través del sistema de estabilidad
- Variabilidad estacional que afecta la jugabilidad
- Balance entre contenido narrativo fijo y exploración procedural
- Progresión natural de dificultad geográfica

---

## I. Sistemas Fundamentales del Mundo

### 1. Cambios Estacionales
**Objetivo:** Crear variabilidad temporal que afecte tanto la exploración como el mapeo.

**Implementación:**
- El mundo cambia visual y funcionalmente según la temporada actual
- Las estaciones progresan con el [[Documentation/🎮 Mecánicas y Sistemas/Temporalidad/Paso del Tiempo\|Paso del Tiempo]] (Invierno → Primavera → Verano → Otoño)
- Cada región responde diferentemente a los cambios estacionales
- Los desafíos de mapeo varían según la estación

**Impacto en Sistemas:**
- Afecta la accesibilidad de ciertas rutas y regiones
- Modifica la visibilidad de [[Documentation/🌍 Mundo/Anclajes de Estabilidad\|Anclajes de Estabilidad]]
- Influye en la velocidad de deterioro de [[Documentation/Mécanicas y Sistemas/Estabilidad\|Estabilidad]]
- Cambia la disponibilidad de recursos y [[Documentation/🌍 Mundo/Puntos de Interés\|Puntos de Interés]]

### 2. Estabilidad Variable por Región
**Objetivo:** Crear priorización natural de exploración y urgencia diferenciada.

**Implementación:**
- Cada región tiene resistencia única a [[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de El Desvanecimiento\|El Desvanecimiento]]
- Las regiones narrativamente importantes tienen mayor estabilidad base
- La estabilidad determina la velocidad de deterioro sin intervención
- Los [[Documentation/🌍 Mundo/Anclajes de Estabilidad\|Anclajes de Estabilidad]] proporcionan puntos de resistencia

**Conexiones:**
- Directamente vinculado al [[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de Estabilidad y Anclajes\|Sistema de Estabilidad y Anclajes]]
- Afectado por el progreso del [[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de Mapeo\|Sistema de Mapeo]]
- Influenciado por el [[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de Conocimiento\|Sistema de Conocimiento]]

---

## II. Arquitectura de Generación del Mundo

### 1. Esquema Continental (Contenido Fijo)
**Propósito:** Garantizar consistencia narrativa y experiencias de alta calidad.

**Características:**
- Masas de tierra construidas manualmente
- Biomas distintivos con identidad única
- [[Documentation/🌍 Mundo/Puntos de Interés\|Puntos de Interés]] claves para la narrativa principal
- Eventos pre-diseñados y secuencias narrativas
- Mayor densidad de [[Documentation/🌍 Mundo/Anclajes de Estabilidad\|Anclajes de Estabilidad]] narrativos

**Criterios de Diseño:**
- Zonas más detalladas y pulidas visualmente
- Consistencia entre diferentes partidas
- Integración natural con contenido procedural circundante

### 2. Plantillas Regionales (Contenido Semi-Procedural)
**Propósito:** Proporcionar variedad controlada con temas consistentes.

**Tipos de Plantillas:**
- Bosque Antiguo: Enfoque en anclajes naturales y ecológicos
- Archipiélagos Volcánicos: Desafíos de navegación y cambios geológicos
- Desiertos Cristalinos: Fenómenos únicos y recursos especializados
- Tundra Fragmentada: Efectos estacionales extremos
- Pantanos Temporales: Cambios dinámicos según época del año

**Implementación:**
- Cada plantilla tiene reglas de generación específicas
- Temas y desafíos consistentes dentro del tipo
- Variaciones procedurales dentro del marco temático

### 3. Relleno Procedural (Contenido Dinámico)
**Propósito:** Crear experiencias únicas y rejugabilidad infinita.

**Elementos Generados:**
- Terrenos y topografía base
- Caminos y rutas de conexión
- [[Documentation/🌍 Mundo/Puntos de Interés\|Puntos de Interés]] menores
- Distribución de recursos
- Anclajes de menor importancia

**Principios:**
- Respeta las restricciones de las plantillas regionales
- Escala dificultad gradualmente
- Mantiene coherencia con biomas adyacentes

---

## III. Sistemas de Implementación Técnica

### 1. Generación por Capas
**Proceso de Construcción:**

1. **Capa Base:** Posicionamiento del esqueleto continental
2. **Capa de Plantillas:** Aplicación de plantillas regionales
3. **Capa Procedural:** Relleno algorítmico respetando restricciones
4. **Capa de Pulido:** Integración y suavizado de transiciones
5. **Capa de Anclajes:** Distribución de puntos de estabilidad

### 2. Reglas de Bioma
**Parámetros por Bioma:**
- Densidad y tipos de vegetación
- Patrones de formación de elevaciones
- Distribución de recursos naturales
- Frecuencia de fenómenos especiales
- Resistencia base a El Desvanecimiento

### 3. Dificultad Gradual
**Implementación:**
- Progresión geográfica desde zonas centrales seguras
- Escalado de complejidad de [[Documentation/🌍 Mundo/Anclajes de Estabilidad\|Anclajes de Estabilidad]]
- Aumento de velocidad de deterioro por distancia
- Mayor densidad de desafíos en regiones exteriores

### 4. Integración Narrativa
**Principios:**
- Localizaciones narrativas mantienen posición fija
- Rutas entre puntos importantes varían entre partidas
- Eventos narrativos se adaptan a la topografía generada
- Coherencia entre lore y geografía procedural

---

## IV. Dinámicas del Mundo

### 1. Mundo Dinámico
**Sistemas de Cambio:**
- Transformaciones estacionales automáticas
- Respuesta a acciones del jugador
- Evolución basada en progreso de mapeo
- Efectos de [[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de El Desvanecimiento\|Sistema de El Desvanecimiento]]

### 2. Visualización de El Desvanecimiento
**Indicadores Visuales:**
- Cambios graduales en estabilidad regional
- Efectos visuales escalados según deterioro
- Indicadores claros de urgencia temporal
- Feedback visual del progreso de mapeo

**Estados de Deterioro:**
- Conectado directamente con [[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de El Desvanecimiento\|Sistema de El Desvanecimiento]]
- Progresión visual clara de 100% a 0% estabilidad
- Efectos que no interfieren con jugabilidad core

---

## V. Áreas que Requieren Expansión

### **CRÍTICAS (Expandir Inmediatamente):**

1. **Especificaciones de Cambios Estacionales**
   - ¿Qué cambios específicos ocurren en cada bioma por estación?
   - ¿Cómo afectan las estaciones a la accesibilidad y navegación?
   - ¿Qué mecánicas de juego cambian estacionalmente?

2. **Definición Detallada de Plantillas Regionales**
   - Especificaciones completas de cada tipo de región
   - Reglas de generación específicas por plantilla
   - Catálogo de desafíos únicos por tipo

3. **Sistema de Dificultad Gradual**
   - Métricas específicas de escalado
   - Cómo se calcula la progresión de dificultad
   - Balance entre desafío y accesibilidad

### **IMPORTANTES (Expandir Después):**

4. **Reglas de Bioma Detalladas**
   - Parámetros técnicos específicos
   - Algoritmos de generación por tipo
   - Interacciones entre biomas adyacentes

5. **Integración con Sistemas de Anclajes**
   - Distribución algorítmica de anclajes
   - Balanceo de densidad por región
   - Conexiones entre anclajes distantes

### **OPCIONALES (Expandir Si Es Necesario):**

6. **Detalles Técnicos de Implementación**
   - Especificaciones de rendimiento
   - Limitaciones técnicas
   - Optimizaciones de generación

---

## VI. Conexiones con Otros Sistemas

- **[[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de El Desvanecimiento\|Sistema de El Desvanecimiento]]:** Mecánica principal que da urgencia al mundo
- **[[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de Estabilidad y Anclajes\|Sistema de Estabilidad y Anclajes]]:** Puntos de resistencia distribuidos geográficamente
- **[[Documentation/🎮 Mecánicas y Sistemas/Temporalidad/Paso del Tiempo\|Paso del Tiempo]]:** Motor de cambios estacionales
- **[[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de Mapeo\|Sistema de Mapeo]]:** Interacción principal del jugador con el mundo
- **[[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de Conocimiento\|Sistema de Conocimiento]]:** Comprensión profunda del mundo generado
- **[[Documentation/🌍 Mundo/Puntos de Interés\|Puntos de Interés]]:** Elementos específicos distribuidos en el mundo
- **[[Documentation/🌍 Mundo/Eventos\|Eventos]]:** Sucesos temporales que afectan regiones específicas