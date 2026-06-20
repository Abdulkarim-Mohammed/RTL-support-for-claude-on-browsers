# إصلاح تداخل النص العربي في Claude.ai

<div dir="rtl">

## المشكلة

عند استخدام Claude.ai بالعربية، تظهر مشكلة تداخل النصوص العربية والإنجليزية — الكلمات الإنجليزية تتحرك من مكانها الصحيح وسط الجملة وتخرب ترتيب الكلام. المشكلة تطال الجمل العادية، والنقاط، والجداول الممزوجة، وحتى نصوص تفكير كلود الداخلية.

**السبب:** واجهة Claude.ai مبنية أساساً للغات LTR، فخوارزمية Unicode BiDi تتعامل مع النصوص المختلطة بشكل خاطئ.

## الحل

حقن CSS مخصص عبر إضافة **Stylus** يصحح اتجاه كل فقرة تلقائياً دون التأثير على أكواد البرمجة.

## طريقة التثبيت

**1. ثبّت إضافة Stylus**

| المتصفح | الرابط |
|---|---|
| Chrome / Edge | https://chromewebstore.google.com/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne |
| Firefox | https://addons.mozilla.org/en-US/firefox/addon/styl-us/ |

**2. افتح محرر Stylus**

- افتح **claude.ai**
- اضغط أيقونة Stylus ← **Write style for claude.ai**
- 
**3. الصق الكود من ملف** [`RTL-support-for-claude.md`](./RTL-support-for-claude.md)
- احفظ التغييرات (Ctrl + S)
-  حدث الصفحة (Ctrl + R)

## ما الذي يصلحه هذا الحل؟

- ✅ الجمل المختلطة (عربي + إنجليزي)
- ✅ النقاط التي تبدأ بمصطلحات إنجليزية
- ✅ الجداول الممزوجة باللغتين
- ✅ نصوص تفكير Claude الداخلية
- ✅ أكواد البرمجة تبقى LTR دون تأثر

![Demo](./claude-rtl-fix-1280p.gif)

> **ملاحظة:** هذا الحل مخصص لـ Claude.ai في المتصفح فقط. إذا تغيّرت أسماء الكلاسات بعد تحديث الموقع، افتح DevTools (F12) وتحقق من الكلاسات الجديدة.

</div>

---

# Arabic Text Fix for Claude.ai

## Problem

When using Claude.ai in Arabic, English words within mixed-language text get misplaced — appearing at the wrong end of the line instead of their correct position. This affects inline sentences, bullet points, mixed-language tables, and even Claude's internal thinking sections.

**Root cause:** Claude.ai's interface is built primarily for LTR languages. The Unicode BiDi algorithm mishandles mixed-direction content without proper CSS directives.

## Solution

Inject custom CSS via the **Stylus** browser extension to automatically correct text direction per paragraph, without affecting code blocks.

## Installation

**1. Install Stylus**

| Browser | Link |
|---|---|
| Chrome / Edge | https://chromewebstore.google.com/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne |
| Firefox | https://addons.mozilla.org/en-US/firefox/addon/styl-us/ |

**2. Open Stylus Editor**

- Open **claude.ai**
- Click the Stylus icon → **Write style for claude.ai**

**3. Paste the CSS from** [`RTL-support-for-claude.md`](./RTL-support-for-claude.md)
- Save (`Ctrl + S`)
- Reload the page (`Ctrl + R`)

## What Does This Fix?

- ✅ Mixed Arabic/English sentences
- ✅ Bullet points starting with English terms
- ✅ Mixed-language tables
- ✅ Claude's internal thinking sections
- ✅ Code blocks remain LTR unaffected

> **Note:** This fix applies to Claude.ai in the browser only. If class names change after a site update, inspect via DevTools (F12) and update accordingly.

---

*Made by Abdulkarim Aljundubi*
