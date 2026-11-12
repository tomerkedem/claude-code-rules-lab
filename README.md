# claude-code-rules-lab

[English](#english) | [עברית](#עברית)

## English

A small, safe scratch project for practicing Claude Code **Rules**: how
`CLAUDE.md` and scoped Rule files load, and the difference between an
instruction and an enforced `deny` permission rule.

This is the hands-on companion to **Claude Code Masterclass**, Lesson 13
(project rules), section 5 ("Practical Rules laboratory"). The lab steps
themselves are taught in the course. This repository only provides the
starting project so you do not have to build it by hand.

### What is inside

```text
CLAUDE.md                  # project instructions
.env                       # invented demo value only
.claude/
  rules/
    general.md             # no paths: loads at launch
    api.md                 # paths: src/api/**/*.ts
src/
  api/users.ts
  ui/button.ts
```

The repository root plays the role of the `rule-lab/` folder from the course.
Everything else you need (the `InstructionsLoaded` hook setting, the
`deny` rule, the log) you create yourself during the labs. They are
intentionally not included.

### Prerequisites

- [Claude Code](https://code.claude.com) installed and signed in.
- Git, and a terminal (bash on macOS/Linux, PowerShell on Windows).
- A text editor.

### How to start

1. Click **Use this template** on GitHub (or clone the repository) and give
   your copy a name, for example `rule-lab`.
2. Open a terminal in that folder (your own copy, never the original public repository).
3. Follow Lab A ("what loads, and when") and Lab B ("instruction versus
   enforcement") in the course.

### Safety

- Work only in this scratch copy, never inside a real project.
- `.env` holds `DEMO_VALUE=not-a-secret`. Do not put real secrets in it.
- The lab log can contain local paths. It is git-ignored; do not commit it.
- When you finish, delete your copy of the folder.

### Relationship to the course

Claude Code behavior can change between versions. If this project and the
course ever differ, follow the course and its current version notes.

### Author and license

Author: Tomer Kedem. Released under the [MIT License](LICENSE).

---

## עברית

פרויקט ניסוי קטן ובטוח לתרגול **Rules** ב-Claude Code: איך `CLAUDE.md` וקובצי
Rule ממוקדי נתיב נטענים, ומה ההבדל בין הוראה לבין כלל `deny` שנאכף.

זהו פרויקט התרגול של **Claude Code Masterclass**, שיעור 13 (כללי פרויקט),
פרק 5 ("מעבדת Rules מעשית"). את שלבי המעבדה לומדים בקורס עצמו. המאגר הזה רק
מספק את פרויקט ההתחלה, כדי שלא תצטרכו לבנות אותו ידנית.

### מה בפנים

```text
CLAUDE.md                  # הוראות הפרויקט
.env                       # ערך הדגמה מומצא בלבד
.claude/
  rules/
    general.md             # בלי paths: נטען בהפעלה
    api.md                 # paths: src/api/**/*.ts
src/
  api/users.ts
  ui/button.ts
```

שורש המאגר ממלא את תפקיד התיקייה `rule-lab/` מהקורס. את כל השאר (הגדרת ה-hook
של `InstructionsLoaded`, כלל ה-`deny` והיומן) אתם יוצרים בעצמכם במהלך
המעבדות, ולכן הם אינם כלולים כאן בכוונה.

### דרישות מקדימות

- [Claude Code](https://code.claude.com) מותקן ומחובר לחשבון.
- Git וטרמינל (bash ב-macOS וב-Linux, PowerShell ב-Windows).
- עורך טקסט.

### איך מתחילים

1. לחצו **Use this template** ב-GitHub (או שכפלו את המאגר) ותנו לעותק שלכם
   שם, למשל `rule-lab`.
2. פתחו טרמינל בתיקייה הזו (העותק שלכם, לא המאגר הציבורי המקורי).
3. עקבו אחרי מעבדה א ("מה נטען, ומתי") ומעבדה ב ("הוראה מול אכיפה") בקורס.

### בטיחות

- עבדו רק בעותק הניסוי הזה, ולעולם לא בתוך פרויקט אמיתי.
- בקובץ `.env` יש רק `DEMO_VALUE=not-a-secret`. אין לשים בו סודות אמיתיים.
- היומן של המעבדה עשוי להכיל נתיבים מקומיים. הוא מוחרג ב-git, ואין להעלות אותו.
- בסיום מחקו את העותק של התיקייה.

### הקשר לקורס

התנהגות של Claude Code עשויה להשתנות בין גרסאות. אם יש הבדל בין הפרויקט הזה
לבין הקורס, פעלו לפי הקורס ולפי הערות הגרסה שלו.

### מחבר ורישיון

מחבר: תומר קדם (Tomer Kedem). מופץ ברישיון [MIT](LICENSE).
