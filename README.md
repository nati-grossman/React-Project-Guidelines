# הנחיות לפרויקט React

אתר סטטי פשוט (HTML + CSS) שמרכז Best Practices, דפוסים (Patterns) וצ'ק־ליסטים לפרויקטי React. האתר מאורגן לפי קטגוריות (Structure & Organization, State Management, Performance & Optimization, Error Handling & Stability, Styling & UI Patterns, Collaboration & Workflow, Testing, API & Data Fetching, Security in React, Build & Deployment) וכל נושא כתוב בעמוד HTML נפרד.

## סקירה כללית

- דף בית: `index.html`
- סגנונות גלובליים: `styles.css`
- לכל קטגוריה תיקייה משלה עם קבצי `.html` עצמאיים
- תמיכה מלאה בעברית (RTL) בעמודים, עם בלוקי קוד ב־LTR לנראות מיטבית

## מבנה הפרויקט

```
React Project Guidelines/
├─ index.html
├─ styles.css
├─ Structure & Organization/
├─ State Management/
├─ Performance & Optimization/
├─ Error Handling & Stability/
├─ Styling & UI Patterns/
├─ Collaboration & Workflow/
├─ Testing/
├─ API & Data Fetching/
├─ Security in React/
└─ Build & Deployment/
```

## הנחיות כתיבה

- שפה וכיוון טקסט:
  - שורש המסמך: `dir="rtl"` עבור עברית.
  - דוגמאות קוד יש לעטוף בתוך `<pre dir="ltr"><code>...</code></pre>` כדי לאכוף כיוון שמאל־לימין.
- שמות קבצים: להשתמש ב־kebab-case ושמות תיאוריים, לדוגמה: `authentication-authorization-user-permissions.html`.
- קישורים מתוך `index.html`:
  - להשתמש בנתיבים יחסיים.
  - להחליף רווחים ב־`%20` בתוך `href` (למשל `Security%20in%20React/...`).
- סגנון:
  - להעדיף שימוש ב־`styles.css` הגלובלי.
  - במידת הצורך, להוסיף סגנון מקומי מצומצם בלבד.

## הוספת וולוג חדש

1. צרו קובץ `.html` חדש בתיקייה של הקטגוריה המתאימה.
2. הגדירו את תגית ה־HTML הראשית כך: `<html lang="he" dir="rtl">`.
3. הוסיפו קישור חזרה לדף הבית: `<a href="../index.html">`.
4. עטפו דוגמאות קוד בתוך `<pre dir="ltr"><code> ... </code></pre>`.
5. עדכנו את `index.html` עם `<li>` וקישור לעמוד החדש.

## תצוגה מקומית (Local Preview)

- אפשרות 1: לפתוח את `index.html` ישירות בדפדפן.
- אפשרות 2: להרים שרת סטטי מקומי:
  - התקינו: `npm i -g serve`
  - הריצו: `serve -s .`

## פריסה (Deployment)

האתר סטטי וניתן לפריסה ב־Netlify, Vercel, GitHub Pages או S3 + CloudFront.

- Netlify: ללא build; ספריית פרסום היא שורש הפרויקט (האתר מוכן מראש).
- Vercel: להשתמש ב־`@vercel/static-build` או להגיש ישירות מהשורש (ללא build).
- GitHub Pages: להפעיל Pages על תיקיית השורש.

## מאגר (Repository)

- GitHub: `https://github.com/nati-grossman/React-Project-Guidelines.git`

## הערות

- לשמור על תוכן תמציתי ומגובה בדוגמאות.
- לוודא שכל קישור ב־`index.html` מצביע לקובץ קיים ולא ריק.
- להקפיד על כללי RTL/‏LTR לטקסט לעומת קוד.
