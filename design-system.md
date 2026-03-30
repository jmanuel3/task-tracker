# Design System — Task Tracker

## Tipografía — Inter Tight (Fontsource)
- H1 — Título app: 24px / 700
- H2 — Sección: 18px / 600
- H3 — Proyecto: 15px / 600
- Body — Tareas: 14px / 400
- Notas: 13px / 400 italic
- Labels / badges: 11px / 500 uppercase
- Fechas / meta: 11px / 400

## Colores — Light mode
- `--color-primary`: #4F46E5
- `--color-primary-hover`: #6366F1
- `--color-accent`: #DB2777
- `--bg-primary`: #F5F3FF
- `--bg-secondary`: #FFFFFF
- `--bg-tertiary`: #EEF2FF
- `--text-primary`: #1E1B4B
- `--text-secondary`: #6B7280
- `--border`: #E5E7EB

## Colores — Dark mode
- `--color-primary`: #818CF8
- `--color-accent`: #F472B6
- `--bg-primary`: #0F0E1A
- `--bg-secondary`: #1A1830
- `--bg-tertiary`: #252340
- `--text-primary`: #E0E7FF
- `--text-secondary`: #A5B4FC
- `--border`: #312E81

## Prioridades
- Alta: #DB2777
- Media: #D97706
- Baja: #059669
- Perfeccionista ✨: #4F46E5

## Tamaños y espaciado
- Sidebar expandido: 220px
- Sidebar colapsado: 50px
- Topbar altura: 52px
- Border radius card: 12px
- Border radius badge: 20px (pill)
- Border radius input: 8px
- Padding card: 16px 20px
- Gap entre tareas: 8px
- Gap entre secciones: 24px
- Checkbox: 16x16px

## Breakpoints responsive
- Móvil: menos de 768px → sidebar oculto, barra inferior, una columna
- Tablet: 768px – 1024px → sidebar colapsado, dos columnas
- Desktop: más de 1024px → sidebar expandido, layout completo

## Efectos de componentes

### Hover flotante en tareas
- Sube 2px + sombra suave índigo
- Transición 150ms ease

### Checkbox completado
- Animación bounce al marcar
- Texto tachado con opacity 0.5
- Transición 300ms ease

### Sidebar item activo
- Fondo bg-tertiary + borde izquierdo 3px primary
- Hover → slide 4px derecha + borde índigo

### Sidebar colapsable
- Expandido: 220px / Colapsado: 50px con puntos de color
- Hover sobre punto colapsado → tooltip con nombre del proyecto
- Transición 200ms ease

### Botón primary
- Hover: opacity + scale(1.02)
- Active: scale(0.98)

### Toggle dark/light
- Transición global 200ms ease en color y background
- Aplicado en `*` para no afectar rendimiento

### Modal nuevo proyecto/tarea
- Fade in + scale 0.95 → 1
- Overlay oscuro 40% opacity
- Se cierra con Escape o clic fuera

## Modal motivacional
- Aparece al completar una tarea
- Tamaño mediano, centrado en pantalla
- Contenido: emoji grande + mensaje + subtexto
- Barra de progreso inferior que indica tiempo restante
- Desaparece solo (duración a definir al codificar)
- Color de barra según prioridad:
  - Alta: #DB2777
  - Media: #D97706
  - Baja: #059669
  - Perfeccionista: #4F46E5
- Mensajes:
  - Alta: 🔥 "¡Brutal! Eso no era fácil."
  - Media: 💪 "¡Buen trabajo! Vas a un ritmo increíble."
  - Baja: ✅ "Pequeños pasos, grandes avances."
  - Perfeccionista: ✨ "¿En serio? ¡Eres un crack!"

## Límites de la app
- Máximo 4 proyectos
- Máximo 20 tareas por proyecto

## Mensajes de error motivadores

### Al alcanzar límite de proyectos (mínimo 3 mensajes distintos)
- "Tranquilo, las cosas se hacen poco a poco. Acaba lo que tienes antes de empezar algo nuevo."
- "Dale importancia a lo importante. Menos proyectos, más foco."
- "Los grandes resultados vienen de enfocarse. Termina uno antes de abrir otro."

### Al alcanzar límite de tareas (mínimo 3 mensajes distintos)
- "Dale prioridad a lo importante. 20 tareas son más que suficientes para avanzar."
- "Menos es más. Completa algunas tareas antes de añadir más."
- "El foco es tu superpoder. Trabaja lo que tienes antes de añadir más."

## Tiempo estimado por prioridad
- Alta: 2 horas
- Media: 1 hora
- Baja: 30 minutos
- Perfeccionista: 3 horas