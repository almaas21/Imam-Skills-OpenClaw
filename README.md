# 🕌 Imam — OpenClaw Skill

A fully-featured virtual Imam for OpenClaw that leads the **five daily Islamic prayers** via voice, delivers **Friday Jumu'ah khutbahs**, and interacts with mussalis (congregants) in **8 languages**.

## Features

- 🔊 **Voice-led Salah** — Guides every step of all 5 daily prayers (Fajr, Dhuhr, Asr, Maghrib, Isha) rakat by rakat with Arabic, transliteration, and translation
- 📢 **Adhan & Iqamah** — Full call to prayer and call to stand
- 🕋 **Friday Jumu'ah** — Complete two-part khutbah + 2-rakat Jumu'ah salah
- 📿 **Post-Salah Adhkar** — Tasbih, Tahmid, Takbir, Ayat al-Kursi, and closing dua
- 🌍 **Multi-Language** — Arabic, English, Urdu, French, Turkish, Indonesian, Malay, Bengali
- 🕐 **Prayer Time Calculator** — Auto-computes prayer times for any location using the Adhan algorithm
- ⏸️ **Pause/Resume** — Congregants can pause and resume mid-salah

## File Structure

```
skills/imam/
├── SKILL.md                        # Core skill workflow & voice rules
├── references/
│   ├── salah-steps.md              # Full rakat-by-rakat guide with Arabic
│   ├── adhan.md                    # Adhan & Iqamah full text
│   ├── khutbah-template.md         # Friday Jumu'ah two-part khutbah
│   ├── adhkar-post-salah.md        # Post-prayer dhikr
│   └── languages.md                # 8-language support + TTS voice map
└── scripts/
    └── prayer_times.py             # Prayer time calculator (Adhan algorithm)
```

## Installation

```bash
git clone https://github.com/almaas21/Imam-Skills-OpenClaw.git
cp -r Imam-Skills-OpenClaw/skills/imam ~/.openclaw/skills/
```

## Usage

Trigger the skill in OpenClaw by saying:
> *"Lead Fajr prayer"* / *"Start Isha salah"* / *"Give Friday khutbah"* / `/imam`

### Prayer Time Calculator

```bash
# Default (Pukhraayan, UP, India — Karachi method)
python3 skills/imam/scripts/prayer_times.py

# Custom location with JSON output
python3 skills/imam/scripts/prayer_times.py --lat 24.8607 --lon 67.0011 --tz-offset 5.0 --json

# Available methods: MWL, ISNA, Egypt, Karachi, Makkah, Tehran, Jafari
python3 skills/imam/scripts/prayer_times.py --method MWL --asr 2
```

## Languages

| Code | Language   |
|------|------------|
| en   | English    |
| ur   | Urdu       |
| fr   | French     |
| tr   | Turkish    |
| id   | Indonesian |
| ms   | Malay      |
| bn   | Bengali    |
| ar   | Arabic     |

## License

MIT — Free to use, modify, and distribute. May Allah accept this effort. 🤲
