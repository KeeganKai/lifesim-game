# LIFESPANS — Terminal v5.6

> A hyper-realistic, AI-driven life simulator. Live an entire life, month by month.

A complete, single-file browser game inspired by lifespans.app. No build step, no server, no login required — just open `index.html` or host on GitHub Pages.

---

## 🚀 Quick Start

### Option A — Open Locally
1. Download or clone this repository
2. Open `index.html` in any modern browser
3. Play immediately (built-in story engine, no API key needed)

### Option B — GitHub Pages (Recommended)
1. Fork or upload this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to **main branch / root**
4. Your game will be live at `https://yourusername.github.io/repo-name`

---

## 🤖 AI Narrator Setup (Optional but Recommended)

The game includes a built-in story engine that works without any API key. For richer, fully dynamic AI-generated stories:

1. Get an OpenAI API key at [platform.openai.com](https://platform.openai.com)
2. When the game loads, click **⚙ SETTINGS** in the top bar
3. Paste your key into **OPENAI API KEY**
4. Choose your model:
   - `gpt-4o-mini` — fast, cheap (~$0.001/turn)
   - `gpt-4o` — smarter, richer stories (~$0.01/turn)
5. Click **[SAVE]**

> Your API key is stored **only in your browser** (localStorage). It never leaves your device except to call OpenAI's API directly.

---

## 🎮 How to Play

### Input
- **Type freely** in the "WHAT DO YOU DO?" box — describe any action
- Press **Enter** or **[GO]** to submit
- Press **A / B / C** keys to instantly pick a preset choice

### Narrator Dialogue
- Wrap text in **(parentheses)** to speak directly to the narrator
- Example: `(why is this happening to me?)`

### Narrator Tone
Click **📖 LITERARY** in the top bar to cycle through tones:
- **LITERARY** — rich, evocative prose
- **BRUTAL** — raw, unflinching honesty
- **CINEMATIC** — action-movie pacing
- **POETIC** — lyrical and introspective
- **MINIMAL** — sparse, factual
- **COMEDIC** — darkly funny

---

## 💾 Save System

The game **auto-saves after every action** to your browser's localStorage. If you close the tab and come back, your game resumes exactly where you left off. Use **[RESUME SAVE]** on the character creation screen.

To wipe your save: **⚙ SETTINGS → [WIPE SAVE]**

---

## ⚡ Cheat Codes

Type any of these into the action input. **Your run will be flagged as a cheat run.**

| Command | Effect |
|---|---|
| `/skip` | Auto-success on next action |
| `/roll20` | Force a natural 20 (spectacular success) |
| `/roll1` | Force a natural 1 (critical failure) |
| `/wealth 500000` | Set bank balance to 500,000 |
| `/stat charisma 18` | Set a stat to exact value |
| `/stats str=20 cha=18` | Set multiple stats at once |
| `/salary 85000` | Lock annual salary at $85,000 |
| `/salary unlock` | Unlock salary (allow AI to change it) |
| `/npc add Name, relation, age, desc` | Add an NPC next turn |
| `/npc remove Name` | Remove an NPC from relationships |
| `/npc delete Name` | Hard-delete an NPC |
| `/max` | Max health, happiness, and $10M balance |
| `/immortal` | Toggle immortality (no health loss, no death until age 100) |
| `/die reason` | Kill your character with optional cause of death |

---

## 🎭 Features

### Character System
- **6 D&D-style Attributes**: STR, DEX, CON, INT, WIS, CHA (1–20)
- Point-buy system during character creation (27 points, max 18 at creation)
- Attributes influence AI story generation
- **7 Historical Eras**: Ancient, Medieval, Renaissance, Industrial, Modern, Contemporary, Near Future
- Era-appropriate names, locations, and currency

### Vitals & Finances
- **Health** and **Happiness** bars (0–100) with color indicators
- **Bank Balance**, **Monthly Income/Expenses**, **Annual Salary**
- Net per month calculation
- Era-appropriate currencies (gold coins → credits)
- Financial tracking across your entire life

### Relationships
- Dynamic NPC list with name, relation, age, description
- NPCs age over time alongside your character
- Partner and children tracking
- AI narrator references your active relationships in stories

### AI Story Engine
- Fully dynamic story generation via OpenAI
- The AI knows your complete game state (attributes, finances, relationships, era)
- Reacts to your typed actions and choices
- Handles narrator dialogue, dice overrides, and cheat flags
- Rolling conversation history (last 10 turns) for story continuity
- Graceful fallback to built-in engine if AI is unavailable

---

## 📁 File Structure

```
lifespans-mirror/
├── index.html    ← Everything. The entire game.
└── README.md     ← This file.
```

Single file. No dependencies. No build tools. Just HTML.

---

## 🌐 Browser Compatibility

Works in all modern browsers:
- Chrome / Edge 88+
- Firefox 85+
- Safari 14+

---

## ⚠️ Notes

- This is a fan-made mirror/clone for educational and personal use
- Original game at [lifespans.app](https://www.lifespans.app)
- The AI narrator requires your own OpenAI API key — usage costs apply per your OpenAI plan
- Save data is browser-local and not synced across devices

---

*"The feeling of sonder: the realization that each passerby has a life as vivid and complex as your own."*
