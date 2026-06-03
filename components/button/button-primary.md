# Button – Primary / Normal / L

## Overview
El botón Primary representa la acción principal dentro de la interfaz.

Esta variante (`Primary / Normal / L`) define el estado base del botón en tamaño grande, utilizando los tokens del sistema de diseño AppFactory.

---

## Estructura

El componente se compone de:

- Contenedor (`button`)
- Texto (`label`)
- Icono opcional (izquierda o derecha)

```html
<button class="btn btn--primary btn--lg">
  <span class="btn__icon btn__icon--left"></span>
  <span class="btn__label">Botón</span>
  <span class="btn__icon btn__icon--right"></span>
</button>
```

## Layout
```css
display: inline-flex;
padding: var(--spacing-sm, 16px);
justify-content: center;
align-items: center;
gap: var(--spacing-2xs, 4px);
```

Alineación centrada (horizontal y vertical)
Permite texto + icono
Espaciado consistente mediante tokens

## Shape

```css
border-radius: var(--components-button-solid-primary-default-border-radius, 12px);
```

## Color

```css
background: var(--components-button-solid-primary-default-background, #224D70);
color: var(--components-button-solid-primary-default-foreground-color, #FFF);
```

## Tipografía

```css
font-family: "Nunito Sans";
font-size: var(--font-size-md, 20px);
font-style: normal;
font-weight: 700;
line-height: var(--line-height-xl, 24px);
text-align: center;
```
## Iconografía

```css
width: 16px;
height: 16px;
```

Posiciones soportadas:
- icono izquierda
- icono derecha

## Ejemplo

```html
<button class="btn btn--primary">
  Botón
  <svg width="16" height="16">
    <!-- icon -->
  </svg>
</button>
```

Comportamiento

Acción principal de la interfaz
Alta visibilidad
No requiere borde adicional
Se utiliza para CTAs


## Tokens implicados

spacing-sm
spacing-2xs
font-size-md
line-height-xl
components-button-solid-primary-default-background
components-button-solid-primary-default-foreground-color
components-button-solid-primary-default-border-radius

## Ejemplo completo

```html
<button class="btn btn--primary btn--lg">
  Botón
</button>
```

```css
.btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: var(--spacing-2xs);
  padding: var(--spacing-sm);
  font-family: "Nunito Sans";
}

.btn--primary {
  background-color: var(--components-button-solid-primary-default-background);
  color: var(--components-button-solid-primary-default-foreground-color);
  border-radius: var(--components-button-solid-primary-default-border-radius);
  font-size: var(--font-size-md);
  font-weight: 700;
  line-height: var(--line-height-xl);
}
```