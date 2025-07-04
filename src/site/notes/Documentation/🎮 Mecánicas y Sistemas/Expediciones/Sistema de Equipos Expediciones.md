---
{"dg-publish":true,"dg-path":"🎮 Mecánicas y Sistemas/Expediciones/Sistema de Equipos Expediciones.md","permalink":"/mecanicas-y-sistemas/expediciones/sistema-de-equipos-expediciones/","dgPassFrontmatter":true}
---


# Sistema de Equipos Expediciones

## Descripción General

El sistema de equipos expediciones permite al jugador enviar especialistas desde su campamento para explorar y confirmar puntos de interés marcados en el mapa. Las expediciones operan en tiempo real mientras el jugador explora, creando un sistema dinámico donde ambas actividades se complementan.

## Pilares de Diseño

- **Especialización:** Cada tipo de equipo tiene fortalezas específicas para diferentes tipos de localizaciones
- **Confirmación de Mapeo:** Los equipos validan y confirman puntos de interés marcados por el jugador
- **Tiempo Real:** Las expediciones ocurren simultáneamente con la exploración del jugador
- **Evolución Progresiva:** Los expedicionarios mejoran sus capacidades con el uso y experiencia
- **Interacción Dinámica:** El jugador puede encontrar y interactuar con sus equipos durante la exploración

## Mecánicas Fundamentales

### Despliegue de Expediciones

**Proceso de Envío:**
1. Seleccionar punto de interés marcado en el mapa
2. Elegir tipo de equipo apropiado para la localización
3. Asignar recursos necesarios (suministros, equipamiento)
4. Confirmar expedición y tiempo estimado

**Factores de Éxito:**
- **Precisión del Mapa:** Certeza de la posición, escala correcta, detalles del terreno
- **Especialización Correcta:** Coincidencia entre tipo de equipo y naturaleza de la localización
- **Recursos Adecuados:** Suministros suficientes para duración y composición del equipo
- **Condiciones Ambientales:** Temporada/clima apropiado para la expedición
- **Conocimiento Previo:** Información disponible sobre la localización objetivo

### Confirmación de Puntos de Interés

**Sistema de Validación:**
- Los equipos llegan a la zona marcada y evalúan si corresponde con su especialidad
- **Match Exitoso:** Punto válido + equipo apropiado = confirmación del punto de interés
- **Fallo de Confirmación:** Si el punto es diferente a lo esperado, la expedición falla sin consecuencias graves
- **Evolución del Sistema:** Expedicionarios experimentados pueden proporcionar información sobre puntos cercanos o corregir errores en el mapa

### Interacción en Tiempo Real

**Encuentros Durante Exploración:**
- Los equipos aparecen en el mundo mientras realizan su trabajo
- **Interacciones Simples:** Burbujas de diálogo con pistas, animaciones o sonidos característicos
- **Reconocimiento Mutuo:** Los equipos saludan o hacen ruidos al ver al jugador
- **Fluidez Constante:** Las interacciones no detienen el flujo del juego

**Control Dinámico:**
- Cambio de órdenes sobre la marcha (redirección a nueva localización)
- Llamar equipos cercanos a la posición del jugador
- Ajustes menores sin interrumpir la expedición principal

## Tipos de Equipos Expedicionarios

### Equipo Botánico
**Especialización:** Flora, propiedades herbarias, ecosistemas vegetales
- **Mejores Para:** Formaciones inusuales de plantas, hierbas medicinales, anomalías forestales
- **Retornan Con:** Semillas raras, conocimiento de plantas, remedios naturales, información ecológica
- **Propósito:** Descubrir plantas con efectos de jugabilidad (curación, buffs)
- **Contribución a Estabilidad:** Identifican patrones vegetales que sirven como anclajes naturales

### Equipo Geológico
**Especialización:** Formaciones rocosas, minerales, análisis de terreno
- **Mejores Para:** Formaciones rocosas extrañas, depósitos minerales, análisis estructural
- **Retornan Con:** Muestras minerales, cristales, mapeo de cuevas, conocimiento estructural
- **Propósito:** Encontrar recursos valiosos para comercio o fabricación de herramientas
- **Contribución a Estabilidad:** Descubren anclajes geológicos que refuerzan la estabilidad regional

### Equipo Mercenario
**Especialización:** Combate, navegación en terrenos peligrosos, evaluación de amenazas
- **Mejores Para:** Territorios con monstruos, campamentos hostiles, terrenos peligrosos
- **Retornan Con:** Rutas seguras, evaluación de peligros, artefactos recuperados, patrones de comportamiento
- **Propósito:** Liberar zonas peligrosas y proteger otras expediciones
- **Contribución a Estabilidad:** Asegurar áreas aumenta la estabilidad local

### Equipo Arqueológico
**Especialización:** Ruinas, artefactos, civilizaciones antiguas
- **Mejores Para:** Ruinas, monumentos, construcciones extrañas, asentamientos antiguos
- **Retornan Con:** Conocimiento histórico, fragmentos de artefactos, información arquitectónica y cultural
- **Propósito:** Descubrir elementos históricos y resolver misterios regionales
- **Contribución a Estabilidad:** Los sitios antiguos contienen anclajes de estabilidad poderosos

### Emisarios Culturales
**Especialización:** Diplomacia, lingüística, interacción con civilizaciones locales
- **Mejores Para:** Villas, puntos de intercambio, sitios culturales, lugares sagrados
- **Retornan Con:** Fragmentos de lenguaje, prácticas culturales, mitos locales, acuerdos comerciales
- **Propósito:** Construir relaciones que abren nuevas oportunidades y misiones
- **Contribución a Estabilidad:** El conocimiento local es clave para identificar nuevos anclajes

### Equipo Naturalista
**Especialización:** Vida salvaje, comportamiento animal, ecosistemas
- **Mejores Para:** Rutas de migración, guaridas de criaturas, anomalías ecosistémicas
- **Retornan Con:** Observaciones de comportamiento, catálogo de especies, técnicas de caza y domesticación
- **Propósito:** Descubrir criaturas con comportamientos únicos que afectan la exploración
- **Contribución a Estabilidad:** Comprender el ecosistema aumenta la estabilidad general

## Sistema de Resultados

### Niveles de Éxito

**Fallo Crítico:**
- Equipo perdido o gravemente herido
- Recursos completamente consumidos
- Reducción de reputación y moral

**Fallo Parcial:**
- Equipo regresa con heridas menores
- Recompensa mínima obtenida
- Pérdida parcial de recursos

**Éxito Básico:**
- Equipo regresa intacto con recompensa esperada
- Confirmación exitosa del punto de interés
- Recursos utilizados según lo planeado

**Éxito Mejorado:**
- Recompensa esperada más descubrimientos adicionales
- Información extra sobre la región
- Eficiencia en el uso de recursos

**Éxito Crítico:**
- Descubrimientos únicos que impactan el mundo
- Revelación de nuevos puntos de interés
- Bonificaciones significativas al conocimiento regional

## Eventos Especiales

### Activación de Anclajes
- Ciertos anclajes requieren presencia de equipos específicos para activarse
- Múltiples expedicionarios pueden ser necesarios para anclajes complejos
- Coordinación entre diferentes tipos de equipos

### Eventos Culturales y Temporales
- Festivales o ceremonias que requieren presencia de Emisarios Culturales
- Eventos estacionales que solo ocurren en condiciones climáticas específicas
- Fenómenos naturales que necesitan observación especializada

### Características de los Eventos
- **Repetibilidad:** La mayoría son repetibles pero con recompensas decrecientes
- **Condiciones:** Pueden requerir clima específico, época del año, o múltiples expediciones
- **Descubrimiento:** Algunos eventos solo se revelan después de confirmar ciertos puntos de interés

## Progresión y Evolución

### Desarrollo de Expedicionarios

**Personalidad por Especialidad:**
- Cada tipo de equipo desarrolla características únicas según su área de expertise
- Los rasgos de personalidad influyen en las interacciones y reportes
- Especialistas experimentados proporcionan información más detallada

**Evolución de Capacidades:**
- Las habilidades mejoran con el uso y experiencia en campo
- Expedicionarios veteranos pueden identificar oportunidades adicionales
- Capacidad progresiva para corregir errores de mapeo y sugerir mejoras

### Mejoras de Equipamiento

**Herramientas Especializadas:**
- Equipamiento mejorado aumenta las posibilidades de éxito
- Herramientas específicas para cada tipo de expedición
- Tecnologías que se desbloquean con el progreso del juego

**Gestión de Recursos:**
- Balanceo progresivo entre costo y beneficio de las expediciones
- Decisiones estratégicas sobre asignación de recursos limitados
- Optimización de rutas y timing para maximizar eficiencia

## Riesgos y Consecuencias

### Amenazas Ambientales
- **El Desvanecimiento:** Expedicionarios pueden perderse en regiones afectadas
- **Heridas y Pérdidas:** Equipos pueden ser heridos o perdidos permanentemente
- **Condiciones Adversas:** Clima y terreno peligroso afectan las posibilidades de éxito

### Gestión de Personal
- **Intercambiabilidad:** Todos los expedicionarios son intercambiables dentro de su categoría
- **Reemplazo:** Sistema de reclutamiento para reponer pérdidas (mecánica a definir)
- **Límites Operacionales:** Restricciones en expediciones simultáneas (balanceo a definir)

## Integración con Otros Sistemas

### Conexiones Principales
- **[[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de Mapeo\|Sistema de Mapeo]]:** Las expediciones validan y mejoran la precisión del mapa
- **[[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de Conocimiento\|Sistema de Conocimiento]]:** Los descubrimientos se registran automáticamente
- **[[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de Campamentos\|Sistema de Campamentos]]:** Base de operaciones para todas las expediciones
- **[[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de El Desvanecimiento\|Sistema de El Desvanecimiento]]:** Riesgo constante que afecta la seguridad de las expediciones
- **[[Documentation/🎮 Mecánicas y Sistemas/Core/Sistema de Estabilidad y Anclajes\|Sistema de Estabilidad y Anclajes]]:** Contribución directa al descubrimiento y activación de anclajes

### Flujo de Información
- Los resultados de expediciones alimentan el sistema de conocimiento
- Las mejoras en el mapa facilitan futuras expediciones
- Los anclajes descubiertos proporcionan bases más seguras para operaciones

---

**Áreas para Expansión Futura:**
- Mecánicas específicas de reclutamiento
- Sistema de nombres y evolución de expedicionarios
- Balanceo de límites operacionales
- Eventos especiales únicos por región
