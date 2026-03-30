# Design System — Task Tracker

## Tipografía
- Fuente: Inter Tight (Fontsource)
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
- Perfeccionista: #4F46E5

## Tamaños
- Sidebar: 220px
- Topbar: 52px
- Border radius card: 12px
- Border radius badge: 20px
- Border radius input: 8px
- Padding card: 16px 20px
- Gap tareas: 8px
- Gap secciones: 24px
- Checkbox: 16x16px

## Efectos
- Botón hover: opacity + scale(1.02) / active: scale(0.98)
- Tarea hover: bg-tertiary, transición 150ms ease
- Checkbox completado: animación scale + texto tachado opacity 0.5
- Sidebar activo: bg-tertiary + border-left 3px primary
- Toggle dark/light: transición global 200ms ease
- Modal: fade in + scale 0.95→1, overlay 40% opacity

## Modal motivacional
- Aparece al completar una tarea
- Tamaño mediano, centrado en pantalla
- Contenido: emoji grande + mensaje + subtexto
- Barra de progreso inferior que indica tiempo restante
- Desaparece solo (duración a definir al codificar)
- Color de barra según prioridad de la tarea:
  - Alta: #DB2777
  - Media: #D97706
  - Baja: #059669
  - Perfeccionista: #4F46E5
- Mensajes (Provisionales):
  - Alta: 🔥 "¡Brutal! Eso no era fácil."
  - Media: 💪 "¡Buen trabajo! Vas a un ritmo increíble."
  - Baja: ✅ "Pequeños pasos, grandes avances."
  - Perfeccionista: ✨ "¿En serio? ¡Eres un crack!"