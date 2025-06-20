# Proyecto 1 - Reloj Digital con Alarma

## Resumen General
Implementación de un reloj digital completo con microcontrolador ATmega328P que incluye:
- Visualización de hora en formato 24h (HH:MM) con 4 displays de 7 segmentos multiplexados
- Sistema de alarma configurable con indicación audible
- Visualización de fecha en formato DD/MM
- Mecanismos de configuración con overflow/underflow
- Parpadeo de separadores cada 500ms
- Control mediante botones con antirebote

## Características Principales

### 1. Sistema de Visualización
- **4 displays multiplexados** para hora/fecha
- **Puntos centrles parpadeantes** (500ms)
- **Indicadores visuales** para modos de configuración
- Conversión digital a 7 segmentos optimizada

### 2. Gestión de Tiempo
- Base de tiempo con **Timer0 e interrupciones**
- Precisión de reloj de pulsera
- Manejo automático de:
  - Horas (00-23 con overflow)
  - Minutos (00-59 con overflow)
  - Fechas (considerando días por mes)

### 3. Sistema de Alarma
- Configuración independiente de hora/minutos
- **Indicación audible** con buzzer
- Visualización del estado de alarma
- Overflow/underflow en configuración

### 4. Interfaces de Control
- **3-5 botones** para:
  - Cambio de modos (hora/fecha/alarma)
  - Ajuste de valores (incremento/decremento)
- Implementación de **antirebote** por hardware/software
- Feedback visual de acciones
