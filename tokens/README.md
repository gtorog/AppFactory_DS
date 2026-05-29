## 🤖 Machine-readable tokens

Los tokens de AppFactory están diseñados para ser consumidos automáticamente.

### Acceso directo

- https://raw.githubusercontent.com/gtorog/AppFactory_DS/main/tokens/apf_color.json
- https://raw.githubusercontent.com/gtorog/AppFactory_DS/main/tokens/apf_tokens_global.json
- https://raw.githubusercontent.com/gtorog/AppFactory_DS/main/tokens/apf_tokens_components.json

### Estructura

Los tokens siguen una estructura jerárquica basada en JSON:

- Nivel 1: categoría (color, spacing, typography)
- Nivel 2: uso (background, text, border, etc.)
- Nivel 3: variante (primary, secondary, etc.)

### Tipos de tokens

Los tokens están estructurados en diferentes niveles:

- **Tokens Globales**  
  Valores puros de radius (none, sm, md, etc), border (none, sm, md, etc), spacing (none, 2xs, 1xs, etc), size (xxs, xs, md, etc), fontSize (3xl, 2xl, etc), lineHeight (5xl, 4xl, etc) y fontFamily (Merriweather, Nunito Sans, etc). Cada uno de estos tokens están enlazados dentro de los components tokens.
  Ejemplo: colores base, tipografías, spacing.

- **Color**  
  Tokens con significado de color dentro del sistema.  
  Ejemplo: `primary_default`, `primary_100`.

- **Component tokens** *(si aplica)*  
  Tokens específicos de componentes concretos.  
  Ejemplo: `card.border-radius`, `checkbox.border-with`.

---

## 🎨 Theming y modos

El sistema está preparado para soportar:

- Temas de color (Blue o Red) -> Principal Blue, alternativo Red
- Modo claro / oscuro (light / dark)

Esto se consigue mediante:

- Uso de variables
- Referencias entre tokens (alias)
- Posibles capas de override

---

## 🔄 Relación con Figma

Los tokens están pensados para integrarse con:

- Variables locales de Figma
- Plugins como Tokens Studio
- Exportación a código

---

## ⚙️ Uso de los tokens

Los tokens deben consumirse como:

- Variables en diseño
- Variables CSS o equivalentes en desarrollo
- Referencias en componentes

❗ Nunca usar valores hardcodeados directamente.

---


### Ejemplo

```json
{
  "blue_light": {
    "Primary": {
      "Primary Default": {
        "value": "#224d70",
        "type": "color",
        "prefix": "apf_color"
      },
      "Primary 100": {
        "value": "#f9fafb",
        "type": "color",
        "prefix": "apf_color"
      },
      "Primary 200": {
        "value": "#eff3f5",
        "type": "color",
        "prefix": "apf_color"
      }
    }
  }
}