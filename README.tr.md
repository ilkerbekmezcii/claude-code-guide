🌍 [English](README.md) | [Türkçe](README.tr.md) | [Español](README.es.md)

# 🤖 Claude Code — Genel Kullanım Kılavuzu

> **Anthropic tarafından geliştirilen, yerel kabuğunuzda çalışan terminal tabanlı kodlama yardımcısı.**

<div align="center">

![Sürüm](https://img.shields.io/badge/version-latest-blue)
![Lisans](https://img.shields.io/badge/license-Proprietary-red)

</div>

---

## 📚 İçindekiler

- [Claude Code Nedir?](#claude-code-nedir)
- [Kurulum](#kurulum)
- [Hızlı Başlangıç](#hızlı-başlangıç)
- [Etkileşimli Mod (TUI)](#etkileşimli-mod-tui)
- [Yapılandırma](#yapılandırma)
- [Slash Komutları](#slash-komutları)
- [Temel Kısayollar](#temel-kısayollar)
- [İpuçları ve Hileler](#ipuçları-ve-hileler)
- [Kaynaklar](#kaynaklar)
- [Hızlı Başvuru Kartı](#hızlı-başvuru-kartı)

---

## Claude Code Nedir?

**Claude Code**, Anthropic tarafından geliştirilen geliştirici odaklı bir komut satırı arayüzü (CLI) aracıdır. Dosyaları incelemek, kod yazmak, düzenlemek ve Git işlemlerini yönetmek için doğrudan terminal üzerinden Claude ile etkileşime geçmenizi sağlar.

---

## Kurulum

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

## Hızlı Başvuru Kartı

```
┌──────────────────────────────────────────────────────────┐
│                🤖 Claude Code Hızlı Başvuru              │
├──────────────────────────────────────────────────────────┤
│                                                          │
│  BAŞLAT                    YÖNET                         │
│  claude          .......  TUI Başlat      /new           │
│  claude "..."    .......  Prompt ile      /clear         │
│  claude --resume .......  Devam et        /compact       │
│                                           /quit          │
│                                                          │
│  EDİTÖR                    KISAYOL TUŞLARI               │
│  Ctrl+J          .......  Yeni satır      Ctrl+C         │
│  Ctrl+G          .......  Dış editör      Ctrl+D         │
│  Ctrl+R          .......  Komut geçmişi   Ctrl+O         │
│                                           Ctrl+L         │
│                                                          │
│  AYARLAR                                                 │
│  /config         .......  Ayarlar Paneli                 │
│  /model          .......  Modeli değiştir                │
│                                                          │
└──────────────────────────────────────────────────────────┘
```
