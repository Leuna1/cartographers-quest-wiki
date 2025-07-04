---
{"dg-publish":true,"dg-path":"Balanceo de riesgo y recursos.md","permalink":"/balanceo-de-riesgo-y-recursos/","dgPassFrontmatter":true}
---


# Balanceo de Riesgo y Recursos

## Resumen Ejecutivo
El sistema de balanceo de riesgo y recursos forma el núcleo económico del juego, creando tensiones estratégicas entre eficiencia, seguridad y progresión. Este documento detalla los bucles de retroalimentación y las decisiones críticas que definen la experiencia del jugador.

## Bucles de Retroalimentación Principal

### 1. Ciclo de Mejora Progresiva
**Concepto**: Mejores mapas → expediciones más exitosas → más conocimiento → mejores técnicas de mapeo

**Implementación**:
- Los mapas de alta calidad aumentan las probabilidades de éxito de las [[Documentation/Mécanicas y Sistemas/Sistema de Expediciones Personales\|expediciones]]
- Las expediciones exitosas generan [[Documentation/Mécanicas y Sistemas/Sistema de Conocimiento\|conocimiento]] específico sobre regiones
- El conocimiento acumulado desbloquea técnicas avanzadas en el [[Documentation/Mécanicas y Sistemas/Sistema de Mapeo\|Sistema de Mapeo]]

**Ejemplo práctico**: Un mapa detallado de una región peligrosa (95% de precisión) permite a una expedición evitar trampas conocidas, resultando en un 40% más de recursos recolectados y conocimiento sobre rutas seguras para futuras expediciones.

### 2. Tensión Tiempo vs. Calidad
**Concepto**: El mapeo exhaustivo aumenta la [[Documentation/Mécanicas y Sistemas/Estabilidad\|Estabilidad]] pero consume tiempo valioso

**Implementación**:
- Mapeo exhaustivo: +15 puntos de estabilidad, 3-4 días de trabajo
- Mapeo rápido: +5 puntos de estabilidad, 1 día de trabajo
- La [[Documentation/Mécanicas y Sistemas/Sistema de Estabilidad y Anclajes\|estabilidad]] determina la resistencia de las regiones al [[Documentation/Conceptos/El Desvanecimiento\|El Desvanecimiento]]

**Ejemplo práctico**: Una región con 50 puntos de estabilidad resiste 10 días adicionales antes de comenzar a desvanecerse, mientras que una con 20 puntos solo resiste 4 días.

### 3. Cobertura vs. Profundidad
**Concepto**: El mapeo rápido permite cubrir más terreno pero proporciona menos estabilidad por región

**Implementación**:
- Estrategia extensiva: Mapear 5 regiones superficialmente (25 puntos de estabilidad total)
- Estrategia intensiva: Mapear 2 regiones exhaustivamente (30 puntos de estabilidad total)
- El [[Documentation/Mécanicas y Sistemas/Sistema de El Desvanecimiento\|Sistema de El Desvanecimiento]] afecta todas las regiones simultáneamente

**Ejemplo práctico**: Durante una crisis de desvanecimiento, tener 5 regiones parcialmente mapeadas puede ser más valioso que 2 regiones completamente mapeadas, ya que ofrece más opciones de evacuación y recursos distribuidos.

## Sistemas de Inversión y Retorno

### 4. Escalado de Calidad de Expediciones
**Concepto**: La calidad de las expediciones aumenta con inversiones pero consume más recursos

**Implementación**:
- Expedición básica: 10 recursos, 60% probabilidad de éxito
- Expedición mejorada: 25 recursos, 80% probabilidad de éxito
- Expedición premium: 50 recursos, 95% probabilidad de éxito
- Los recursos incluyen suministros, equipamiento y personal especializado

**Ejemplo práctico**: Una expedición premium a una región de alto valor (artefactos raros) justifica la inversión de 50 recursos si el retorno esperado es de 80+ recursos, considerando la alta probabilidad de éxito.

## Presión Temporal y Decisiones Estratégicas

### 5. Impacto de El Desvanecimiento
**Concepto**: La presión de [[Documentation/Conceptos/El Desvanecimiento\|El Desvanecimiento]] genera decisiones estratégicas entre mapeo exhaustivo o mapeo rápido

**Implementación**:
- El Desvanecimiento avanza 1 punto por día en todas las regiones activas
- Regiones con estabilidad <10 puntos entran en "zona crítica"
- Regiones con estabilidad 0 se desvanecen permanentemente
- El jugador debe priorizar qué regiones salvar y cuáles sacrificar

**Ejemplo práctico**: Con 3 regiones en zona crítica y recursos limitados, el jugador debe decidir si:
- Salvar 1 región completamente (mapeo exhaustivo)
- Estabilizar las 3 regiones temporalmente (mapeo rápido)
- Abandonar 1 región para asegurar las otras 2

### 6. Adaptabilidad y Replanificación
**Concepto**: Los [[Documentation/Mécanicas y Sistemas/Mecanismos Anti-Repetición/Eventos de Mundo Dinámicos\|eventos dinámicos]] fuerzan la redistribución de recursos y re-priorización

**Implementación**:
- Eventos aleatorios cada 5-7 días que afectan regiones específicas
- Tipos de eventos: tormentas de desvanecimiento, descubrimientos arqueológicos, bloqueos de rutas
- Cada evento requiere respuesta inmediata y reajuste de estrategia

**Ejemplo práctico**: Un evento de "tormenta de desvanecimiento" acelera la pérdida de estabilidad en una región por 3 días. El jugador debe decidir si:
- Enviar una expedición de emergencia (alto costo, alto riesgo)
- Acelerar el mapeo de esa región (recursos concentrados)
- Evacuar recursos valiosos antes de que se desvanezca

## Métricas de Balanceo para Desarrollo

### Ratios Objetivo
- **Tiempo de mapeo exhaustivo vs. rápido**: 3:1 a 4:1
- **Costo de expedición premium vs. básica**: 5:1 con retorno 2.5:1
- **Tasa de generación de estabilidad vs. pérdida por desvanecimiento**: 1.2:1 en condiciones normales

### Puntos de Decisión Críticos
- Cada 3-4 días: Evaluación de prioridades de mapeo
- Cada 7 días: Revisión de estrategia de expediciones
- Eventos dinámicos: Replanificación inmediata

## Conexiones con Otros Sistemas
- [[Documentation/Mécanicas y Sistemas/Sistema de Campamentos\|Sistema de Campamentos]]: Puntos de apoyo para expediciones
- [[Documentation/Mécanicas y Sistemas/Sistema de Progresión\|Sistema de Progresión]]: Desbloqueo de técnicas avanzadas
- [[Documentation/Mécanicas y Sistemas/Sistema de Equipos Expediciones\|Sistema de Equipos Expediciones]]: Optimización de recursos
- [[Anclajes de Estabilidad\|Anclajes de Estabilidad]]: Herramientas para gestión de estabilidad
