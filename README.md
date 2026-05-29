# AppFactory Design System (AppFactory_DS)

Este repositorio contiene la evolución del sistema de diseño AppFactory, con foco en la tokenización de los estilos visuales para soportar escalabilidad, consistencia y theming (multi-marca y modo oscuro).

## 🎯 Objetivo

Centralizar todas las decisiones de diseño en un sistema basado en **Design Tokens**, que actúe como fuente única de verdad (single source of truth) para:

- Diseño (Figma / variables)
- Desarrollo (web / mobile)
- Documentación y automatización

---

## 📁 Estructura del repositorio

## 🔗 Acceso directo a tokens

Los tokens del sistema pueden consultarse directamente aquí:

- [Ver carpeta tokens](https://github.com/gtorog/AppFactory_DS/tree/main/tokens)

### Archivos principales

- [Colores](https://raw.githubusercontent.com/gtorog/AppFactory_DS/main/tokens/apf_color.json)
- [Tokens components](https://raw.githubusercontent.com/gtorog/AppFactory_DS/main/tokens/apf_tokens_components.json)
- [Tokens Global](https://raw.githubusercontent.com/gtorog/AppFactory_DS/main/tokens/apf_tokens_global.json)

La carpeta `tokens` contiene los **design tokens del sistema**, organizados para facilitar su uso tanto en diseño como en desarrollo.

---

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

- Tema por defecto (Blue)
- Tema alternativo (Red)
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

## 🧠 Importante para herramientas y automatización

Este repositorio está diseñado para ser interpretado por sistemas automáticos (AI agents, pipelines, etc.).

Reglas:

- Los tokens están definidos en formato estructurado (JSON u otro equivalente)
- Los nombres siguen una convención semántica
- Los valores pueden referenciar otros tokens (alias)

Esto permite:

- Generación automática de estilos
- Sincronización entre design y code
- Escalabilidad del sistema

---

## 🚀 Roadmap

- [ ] Definición completa de tokens semánticos
- [ ] Integración con Figma Variables
- [ ] Generación automática de CSS / código
- [ ] Soporte completo para theming dinámico
- [ ] Documentación de uso en componentes

---

## 📌 Contexto

AppFactory es el sistema de diseño orientado a la creación de aplicaciones móviles para la Administración Pública, con foco en:

- Accesibilidad
- Consistencia
- Escalabilidad
- Eficiencia en desarrollo

Este repositorio refleja su evolución hacia un modelo basado en Design Tokens.