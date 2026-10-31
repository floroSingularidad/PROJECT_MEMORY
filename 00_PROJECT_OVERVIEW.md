
# PROJECT_CONTEXT
# Operación Submundo

**Documento:** Contexto global del proyecto  
**Versión del documento:** 1.0  
**Estado:** En construcción  
**Última actualización:** 31/10/2026

---

## 1. IDENTIDAD DEL PROYECTO

**Nombre:** Operación Submundo

**Motor:** Godot Engine 4.7.2

**Lenguaje:** GDScript

**Género:** Simulación económica, gestión criminal y estrategia táctica.

**Inspiración principal:** Gangsters: Organized Crime (1998).

**Tipo de proyecto:** Juego de estrategia y gestión para un jugador.

## 2. VISIÓN GENERAL

Operación Submundo es un videojuego de estrategia y gestión en el que el jugador dirige una organización criminal.

El objetivo es construir, desarrollar y controlar una organización clandestina mediante la gestión de personas, recursos económicos, territorios e información.

El juego busca recuperar y ampliar las posibilidades de los antiguos simuladores de gestión criminal, incorporando sistemas interconectados y una mayor profundidad estratégica.

La experiencia debe combinar:

- Gestión de una organización.
- Planificación de operaciones.
- Administración económica.
- Reclutamiento y dirección de agentes.
- Expansión territorial.
- Relaciones con otras organizaciones.
- Investigación y presión policial.
- Consecuencias de las decisiones del jugador.

## 3. PILARES DE DISEÑO

### 3.1. Gestión organizativa

El jugador debe administrar una estructura criminal con diferentes agentes, responsabilidades y funciones.

### 3.2. Economía

Los recursos económicos deben ser fundamentales para mantener y ampliar la organización.

### 3.3. Control territorial

La ciudad debe funcionar como un espacio estratégico dividido en distritos.

### 3.4. Información y riesgo

Las operaciones deben tener consecuencias. La actividad criminal genera sospechas y presión policial.

### 3.5. Estrategia

El jugador debe planificar sus acciones, distribuir recursos y tomar decisiones con información imperfecta.

## 4. ESTRUCTURA GENERAL DEL JUEGO

El diseño contempla dos grandes ámbitos:

**OFICINA**
- Gestión de la organización.
- Administración económica.
- Selección de agentes.
- Planificación de órdenes.
- Gestión estratégica.

**CIUDAD**
- Representación del entorno urbano.
- Distritos y territorios.
- Ejecución de operaciones.
- Actividad de agentes.
- Eventos y consecuencias.

La arquitectura debe mantener separadas estas responsabilidades.

## 5. ARQUITECTURA TÉCNICA

La arquitectura prevista utiliza módulos independientes.

Componentes y sistemas contemplados en el diseño técnico:

- FSM de Hoods: máquina de estados de los agentes.
- GameEvents: comunicación mediante eventos.
- CapitalManager: administración del capital.
- Heat por distrito: sistema de sospecha y presión policial.
- SaveManager: guardado y carga mediante JSON.
- HUD reactivo: interfaz que responde a los cambios del juego.

La implementación concreta de cada componente deberá verificarse en el código fuente.

## 6. ESTADO DEL DESARROLLO

**Versión del juego:** 0.1 (referencia inicial).

**Estado general:** Core y prototipo en desarrollo.

Los sistemas anteriores forman parte de la arquitectura técnica definida, pero su estado de implementación y funcionamiento debe comprobarse en el proyecto Godot.

No considerar un sistema terminado hasta que:
1. Exista su implementación.
2. Se integre correctamente.
3. Se pruebe dentro del motor.
4. Se documenten sus resultados.

## 7. TECNOLOGÍAS Y HERRAMIENTAS

- Godot Engine 3.5.3.
- GDScript.
- Formato de escenas y recursos nativo de Godot.
- Guardado de datos mediante JSON.
- Git para control de versiones.
- ChatGPT como asistente de análisis, programación y documentación.

## 8. REGLAS DE TRABAJO PARA LA IA

ChatGPT debe actuar como programador y arquitecto técnico del proyecto.

Reglas obligatorias:

1. Leer la documentación antes de realizar modificaciones.
2. Analizar el código existente antes de crear sistemas nuevos.
3. Respetar la arquitectura modular.
4. No duplicar funcionalidades existentes.
5. Mantener compatibilidad con Godot 3.5.3.
6. Utilizar GDScript.
7. Explicar los archivos creados y modificados.
8. Evitar modificaciones innecesarias.
9. No considerar terminado un sistema sin verificarlo.
10. Actualizar la documentación después de cada sesión.
11. Registrar las decisiones técnicas importantes.
12. Mantener coherencia entre diseño, arquitectura y código.

## 9. DOCUMENTACIÓN DEL PROYECTO

La documentación se organiza en los siguientes archivos:

- PROJECT_CONTEXT.md: contexto global.
- 00_PROJECT_OVERVIEW.md: visión y objetivos.
- 01_GAME_DESIGN.md: diseño y mecánicas.
- 02_ARCHITECTURE.md: arquitectura técnica.
- 03_CODE_INDEX.md: inventario del código.
- 04_CURRENT_STATUS.md: estado de implementación.
- 05_DECISIONS.md: decisiones técnicas.
- 06_CHANGELOG.md: historial de modificaciones.
- 07_NEXT_TASKS.md: próximas tareas.

## 10. OBJETIVO A LARGO PLAZO

Desarrollar un videojuego de estrategia y gestión criminal profundo, modular y ampliable.

El proyecto debe permitir incorporar nuevas mecánicas, sistemas económicos, agentes, territorios y acontecimientos sin tener que reconstruir continuamente su arquitectura.

La prioridad es construir una base técnica sólida que permita evolucionar el juego progresivamente.

