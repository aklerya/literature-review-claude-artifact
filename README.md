# Literature Review Tool — Claude Artifact (POC v0.1)

**עברית | English below**

> **Proof of concept only.** This is not yet a literature-review engine. It generates three research subquestions with Claude, but does not search academic databases, verify evidence, produce citations, save surveys, or export research reports.

## התחלה מהירה — יצירת עותק אישי ב־Claude

נדרש חשבון [Claude](https://claude.ai/) שתומך ב־Artifacts. אפשר לנסות גם בחשבון חינמי, בכפוף למגבלות השימוש. אין צורך בהתקנת Python או במפתח API נפרד.

1. **הורידו את [קובץ האפליקציה (HTML)](Claude_Artifact_C0_GitHub_Upload_5_Files_v0.1/literature-review-artifact.html)**: פתחו את הקישור, ולחצו ב־GitHub על **Download raw file** (סמל ההורדה). אין צורך לפתוח את הקובץ בדפדפן.
2. פתחו **[שיחה חדשה ב־Claude](https://claude.ai/)** וצרפו את קובץ ה־HTML באמצעות כפתור **+**.
3. העתיקו והדביקו את ההוראה הבאה לשיחה:

> Create a new **private, interactive HTML Artifact** from the attached literature-review-artifact.html file. Preserve its UI, English/Hebrew RTL support, loading/error states and real Claude-powered generation through the Artifact runtime. The **Generate Research Subquestions** button must invoke **real Claude AI**, not mock responses, and generate exactly three topic-specific subquestions. No separate API key, backend, database, academic search, or fictional citations. Show a working interactive preview. If unsupported in this account, explain the limitation instead of simulating success.

4. פתחו את ה־Artifact החדש, הזינו שאלת מחקר ולחצו **Generate Research Subquestions**. אם מופיעה הרשאת **Use Claude**, ודאו שמקור הקובץ הוא המאגר הנכון ואשרו רק אם אתם סומכים עליו. השימוש נספר במכסת Claude של החשבון.

**דוגמה בעברית:** מהם האתגרים הטכנולוגיים העיקריים בהנעה חשמלית ללוויינים קטנים?

**חשוב:** פתיחת קובץ ה־HTML ישירות ב־GitHub או בדפדפן לא תפעיל Claude AI. יש ליצור ממנו Artifact בתוך Claude.

**סטטוס הניסוי:** הצלחנו ליצור Artifact מקובץ ה־HTML ולהפעיל AI באנגלית ובעברית בחשבון אחד. **עדיין לא בדקנו את התהליך בחשבון עצמאי של משתמש נוסף.**

## English — Quick start

Requirements: A [Claude](https://claude.ai/) account supporting Artifacts (a Free account may work within usage limits). No Python installation or separate Anthropic API key is required.

1. Open the [Artifact HTML file](Claude_Artifact_C0_GitHub_Upload_5_Files_v0.1/literature-review-artifact.html) and click **Download raw file** on GitHub.
2. Open a **new chat** at [claude.ai](https://claude.ai/) and attach the downloaded HTML using **+**.
3. Paste the English instruction in the Hebrew quick start above (or use the [full recreation prompt](Claude_Artifact_C0_GitHub_Upload_5_Files_v0.1/CLAUDE_RECREATE_PROMPT.md)).
4. Open your newly created private Artifact. Enter a research question, click **Generate Research Subquestions**, and approve the **Use Claude** permission only if you trust the source. Usage counts toward your Claude account limits.

**Example:** What are the main challenges of autonomous satellite navigation?

Opening the HTML directly as a standalone webpage will **not** activate the Claude integration. Recreation in another independent user's account has **not yet been verified**.

## Repository files / קבצים

All source and setup files are located in the [POC package folder](Claude_Artifact_C0_GitHub_Upload_5_Files_v0.1/).

| File | Purpose |
| --- | --- |
| [literature-review-artifact.html](Claude_Artifact_C0_GitHub_Upload_5_Files_v0.1/literature-review-artifact.html) | Artifact source / קוד המקור |
| [CLAUDE_RECREATE_PROMPT.md](Claude_Artifact_C0_GitHub_Upload_5_Files_v0.1/CLAUDE_RECREATE_PROMPT.md) | Full recreation prompt / הוראה מלאה |
| [CLAUDE_SETUP_HE.md](Claude_Artifact_C0_GitHub_Upload_5_Files_v0.1/CLAUDE_SETUP_HE.md) | Detailed Hebrew setup / מדריך בעברית |
| [TEST_CHECKLIST.md](Claude_Artifact_C0_GitHub_Upload_5_Files_v0.1/TEST_CHECKLIST.md) | Independent validation checklist / בדיקות |
| [VERSION.txt](Claude_Artifact_C0_GitHub_Upload_5_Files_v0.1/VERSION.txt) | Version / גרסה |

## Limitations, privacy and next steps / מגבלות ופרטיות

- The current POC generates **research subquestions only**; it does not perform literature searches or validate citations. AI responses are **not evidence**.
- Research questions are processed by Claude. **Do not submit confidential or restricted research information** without appropriate authorization.
- Review permission prompts; do not share personal API keys or authorize unrelated connectors.
- Updating GitHub **does not automatically update** Artifacts that other users have already recreated.
- This is an experimental distribution method, **not a production-ready release**.

**Next validation:** Ask an independent Claude user to follow these steps, without assistance, and complete the [test checklist](Claude_Artifact_C0_GitHub_Upload_5_Files_v0.1/TEST_CHECKLIST.md). Record whether the Artifact was created and ran AI in English and Hebrew, plus any errors or subscription requirements.
