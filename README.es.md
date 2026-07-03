🌍 [English](README.md) | [Türkçe](README.tr.md) | [Español](README.es.md)

# 🤖 Claude Code — Guía General de Usuario

> **El asistente de codificación basado en terminal desarrollado por Anthropic que se ejecuta en su shell local.**

<div align="center">

![Versión](https://img.shields.io/badge/version-latest-blue)
![Licencia](https://img.shields.io/badge/license-Proprietary-red)

</div>

---

## 📚 Tabla de Contenidos

- [¿Qué es Claude Code?](#qué-es-claude-code)
- [Instalación](#instalación)
- [Inicio Rápido](#inicio-rápido)
- [Modo Interactivo (TUI)](#modo-interactivo-tui)
- [Configuración](#configuración)
- [Comandos de Barra Diagonal](#comandos-de-barra-diagonal)
- [Atajos de Teclado Esenciales](#atajos-de-teclado-esenciales)
- [Consejos y Trucos](#consejos-y-trucos)
- [Recursos](#recursos)
- [Tarjeta de Referencia Rápida](#tarjeta-de-referencia-rápida)

---

## ¿Qué es Claude Code?

**Claude Code** es una herramienta de interfaz de línea de comandos (CLI) centrada en el desarrollador creada por Anthropic. Le permite interactuar con Claude directamente en su terminal para escribir, editar y refactorizar código, inspeccionar archivos y realizar operaciones de Git.

---

## Instalación

### 🪟 Windows (WinGet)
```powershell
winget install Anthropic.ClaudeCode
```

### 🪟 Windows (PowerShell)
```powershell
irm https://claude.ai/install.ps1 | iex
```

### 🍎 macOS / 🐧 Linux
```bash
curl -fsSL https://claude.ai/install.sh | bash
```

---

## Tarjeta de Referencia Rápida

```
┌──────────────────────────────────────────────────────────┐
│             🤖 Referencia Rápida de Claude Code          │
├──────────────────────────────────────────────────────────┤
│                                                          │
│  INICIAR                   GESTIONAR                     │
│  claude          .......  Iniciar TUI     /new           │
│  claude "..."    .......  Con prompt      /clear         │
│  claude --resume .......  Continuar       /compact       │
│                                           /quit          │
│                                                          │
│  EDITOR                    ATAJOS                        │
│  Ctrl+J          .......  Nueva línea     Ctrl+C         │
│  Ctrl+G          .......  Editor externo  Ctrl+D         │
│  Ctrl+R          .......  Historial       Ctrl+O         │
│                                           Ctrl+L         │
│                                                          │
│  CONFIGURACIÓN                                           │
│  /config         .......  Panel de Ajustes               │
│  /model          .......  Cambiar modelo                 │
│                                                          │
└──────────────────────────────────────────────────────────┘
```
