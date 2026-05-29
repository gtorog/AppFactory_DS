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