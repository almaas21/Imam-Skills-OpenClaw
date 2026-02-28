# Multi-Language Support

Arabic recitations are ALWAYS in Arabic regardless of language setting.  
Language preference applies to: instructions, translations, announcements, and khutbah body.

## Supported Languages

| Code | Language   | Prayer Announcement Example                          |
|------|------------|------------------------------------------------------|
| en   | English    | "It is time for Fajr prayer. Let us begin."          |
| ur   | Urdu       | "فجر کی نماز کا وقت ہو گیا ہے۔ شروع کرتے ہیں۔"     |
| fr   | French     | "C'est l'heure de la prière Fajr. Commençons."       |
| tr   | Turkish    | "Sabah namazı vakti geldi. Başlayalım."              |
| id   | Indonesian | "Sudah waktunya shalat Subuh. Mari kita mulai."      |
| ms   | Malay      | "Sudah tiba waktu solat Subuh. Jom kita mulakan."    |
| bn   | Bengali    | "ফজরের নামাজের সময় হয়েছে। শুরু করি।"              |
| ar   | Arabic     | "حان وقت صلاة الفجر. لنبدأ."                         |

## Language Setting Commands
- User says: "Switch to Urdu" → set lang=ur
- User says: "Use English" → set lang=en
- Default: English (en) if not set

## TTS Voice Recommendations (per language)
- Arabic: Use a voice trained on Quranic recitation (e.g., ar-SA-HamedNeural on Azure TTS)
- Urdu: ur-PK-AsadNeural
- English: en-US-GuyNeural (calm, measured tone)
- French: fr-FR-HenriNeural
- Turkish: tr-TR-AhmetNeural
- Indonesian: id-ID-ArdiNeural
- Malay: ms-MY-OsmanNeural
- Bengali: bn-BD-NabanitaNeural
