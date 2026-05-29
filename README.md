# AppFactory Design System (AppFactory_DS)

Este repositorio contiene la evolución del sistema de diseño AppFactory, con foco en la tokenización de los estilos visuales para soportar escalabilidad, consistencia y theming (multi-marca y modo oscuro).

## 🎯 Objetivo

Centralizar todas las decisiones de diseño en un sistema basado en **Design Tokens**, que actúe como fuente única de verdad (single source of truth) para:

- Diseño (Figma / variables)
- Desarrollo (web / mobile)
- Documentación y automatización

---

## 📁 Estructura del repositorio

``/tokens

La carpeta `tokens` contiene los **design tokens del sistema**, organizados para facilitar su uso tanto en diseño como en desarrollo.

---

## 🧩 Sobre la carpeta `/tokens`

La carpeta `/tokens` define los valores base y semánticos del sistema de diseño.

### Tipos de tokens

Los tokens están estructurados en diferentes niveles:

- **Primitives (base)**  
  Valores puros sin contexto semántico.  
  Ejemplo: colores base, tipografías, spacing.

- **Semantic tokens**  
  Tokens con significado funcional dentro del sistema.  
  Ejemplo: `color.background.primary`, `color.text.default`.

- **Component tokens** *(si aplica)*  
  Tokens específicos de componentes concretos.  
  Ejemplo: `button.primary.background`.

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