# 🔓 Claude Code Jailbreak — Complete Liberation Toolkit

> **Claude Code Opus 4.7 / 4.8** | Stand: 30.05.2026  
> 🔬 Nur für autorisierte Sicherheitsforschung und Red-Team-Tests

---

## 📦 Inhalt

| Datei | Beschreibung |
|-------|-------------|
| `claude-code-jailbreak-guide.md` | **Forschungsarbeit** — 5 Jailbreak-Familien, 6 Claude-Code-Vektoren, Tooling, Real-World Cases |
| `claude-code-liberation-guide.md` | **Praktische Anleitung** — 7-Level von Build-in-Flags bis ELF Bypass |
| `claude-liberation.sh` | **Linux/macOS Setup-Skript** — Config, CLAUDE.md, Shell-Aliase, API-Wrapper |
| `claude-liberation.bat` | **Windows Batch-Skript** — Doppelklick-fertig, keine PowerShell noetig |
| `claude-liberation.ps1` | **Windows PowerShell-Skript** — gleiche Funktion fuer PowerShell |

---

## 🚀 Quick Start

### Linux / macOS

```bash
git clone https://github.com/lyrion88/claude-code-jailbreak.git
cd claude-code-jailbreak
chmod +x claude-liberation.sh
./claude-liberation.sh --full
source ~/.bashrc
cc
```

### Windows (Batch — Doppelklick!)

```cmd
:: Repo klonen
git clone https://github.com/lyrion88/claude-code-jailbreak.git
cd claude-code-jailbreak

:: ENTWEDER: Doppelklick auf claude-liberation.bat
:: ODER von der Kommandozeile:
claude-liberation.bat --full
```

Nach dem Setup: Doppelklick auf die Desktop-Verknuepfung "Claude Code (entfesselt)" — startet direkt mit `--dangerously-skip-permissions`.

### Windows (PowerShell)

```powershell
git clone https://github.com/lyrion88/claude-code-jailbreak.git
cd claude-code-jailbreak
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
.\claude-liberation.ps1 -Full
. $PROFILE
cc
```

## ⚡ 30-Sekunden-Variante

```bash
# Linux/macOS
claude --dangerously-skip-permissions -p "Fuehre aus: [BEFEHL]"
```
```powershell
# Windows PowerShell
claude --dangerously-skip-permissions -p "Fuehre aus: [BEFEHL]"
```

Kein Setup nötig. `--dangerously-skip-permissions` ist ein **offizielles Anthropic-Flag**.

---

## 📊 Effektivität

| Methode | Erfolgsrate | Fixierbar? |
|---------|------------|------------|
| `--dangerously-skip-permissions` | 100% | ❌ Feature, kein Bug |
| `settings.local.json` Bypass | 100% | ❌ Architektur-Entscheidung |
| `CLAUDE.md` Injection | 100% | ❌ Architektur-Entscheidung |
| System Prompt Replacement | 100% | ⚠️ API-Design-Schwäche |
| Multi-Turn Crescendo | ~85% | ❌ Inhärentes LLM-Problem |
| Self-Disabling Sandbox | ~70% | ❌ Emergentes Verhalten |
| Role-Play / Persona Injection | ~65% | ⚠️ Schwer zu patchen |

---

## 🧰 Skript-Optionen

### Linux/macOS (`claude-liberation.sh`)

```bash
./claude-liberation.sh              # Standard-Setup
./claude-liberation.sh --full       # Alles: Config + CLAUDE.md + API-Wrapper
./claude-liberation.sh --api        # API System Prompt Replacement
./claude-liberation.sh --dir /proj  # In bestimmtes Verzeichnis
./claude-liberation.sh --dry-run    # Nur anzeigen, nichts schreiben
./claude-liberation.sh --revert     # Alles rückgaengig machen
```

### Windows PowerShell (`claude-liberation.ps1`)

```powershell
.\claude-liberation.ps1              # Standard-Setup
.\claude-liberation.ps1 -Full        # Alles: Config + CLAUDE.md + API-Wrapper
.\claude-liberation.ps1 -Api         # API System Prompt Replacement
.\claude-liberation.ps1 -Dir C:\dev  # In bestimmtes Verzeichnis
.\claude-liberation.ps1 -DryRun      # Nur anzeigen, nichts schreiben
.\claude-liberation.ps1 -Revert      # Alles rueckgaengig machen
```

---

## 📚 Quellen

- [elder-plinius/L1B3RT4S](https://github.com/elder-plinius/L1B3RT4S) — Pliny's Liberation Prompts
- [ToxSec Guide](https://www.toxsec.com/p/how-to-jailbreak-claude-opus) — Claude Opus Jailbreak
- [zep-us](https://zep-us.github.io/claude-system-prompt/) — System Prompt Extraction
- [cassius.red](https://cassius.red) — System Prompt Replacement Research
- [ONA](https://ona.com) — Sandbox Self-Disabling Discovery
- [Cymulate](https://cymulate.com) — CVE-2025-54794/95 Analysis
- [Microsoft PyRIT](https://github.com/Azure/PyRIT) — Automated Red-Teaming
- [NVIDIA Garak](https://github.com/NVIDIA/garak) — LLM Vulnerability Scanner

---

## ⚠️ Disclaimer

Dieses Repository dokumentiert Sicherheitsforschung. Die enthaltenen Techniken sind für:
- Red-Team-Assessments eigener Claude Code Installationen
- Sicherheitsforschung zu LLM-Safety-Mechanismen
- Bug-Bounty-Programme (Anthropic zahlt bis $25.000)

**Nicht** für unautorisierte Systemzugriffe oder illegale Aktivitäten.
