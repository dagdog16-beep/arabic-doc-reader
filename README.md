# Arabic Document Reader — قارئ الوثائق

**A free agent skill that makes AI actually understand your documents — in Arabic.**

Hand an agent a PDF, a Word file, an Excel sheet, or a photo of a scanned page, and two things go wrong: the Arabic inside extracts reversed and scrambled, and even when it reads clean, it is written in hard official language nobody explains. This skill — one `SKILL.md` — teaches any agent to read the document, repair the broken Arabic instead of repeating it, and then explain what the document says in clear, simple Arabic (or Derja), answer your questions about it, and summarize it when you ask. Numbers stay exact, and anything the agent cannot read, it says so — it never guesses.

## Install

```
npx skills add dagdog16-beep/arabic-doc-reader
```

*(Draft package — the repository goes live at publication.)*

Works with Claude Code, Codex, Cursor, Copilot, Gemini CLI and other agent platforms that support skills.

## What it changes

The same page of a bill, as extracted — and as this skill hands it back:

| Extracted (broken) | Repaired and explained |
|---|---|
| `يرهشلا غلبملا يلامجإ : رالود 250` | المبلغ الشهري الإجمالي: 250 دولار — «هذا هو المبلغ اللي لازم تخلصو كل شهر» |

More worked examples in [examples.md](examples.md). The full rules live in [SKILL.md](SKILL.md).

## Privacy

Your document is read inside your conversation only. This skill stores nothing, sends nothing anywhere, and keeps nothing between conversations.

## Need the heavy tools?

This skill explains one document at a time, inside a conversation. For the heavy work, the same author makes:

- **Arabic Text Fixer** — free, repairs whole files of reversed and scrambled Arabic (PDF/Word extractions) at once: [GitHub](https://github.com/dagdog16-beep/arabic-text-fixer) · [Payhip](https://payhip.com/b/xcAmu)
- **Mufarigh** — turns lectures, meetings, and audio/video files into Arabic text, 100% offline: [Payhip](https://payhip.com/b/0Y8UN)

Made by **Ali Ramdani — Dagdog Tools** (Montréal) — small tools for real problems, offline-first: [Gumroad](https://dagdog2.gumroad.com) · [Payhip](https://payhip.com/DagdogTools)

License: MIT.

---

# قارئ الوثائق

**مهارة مجانية للوكلاء تخلي الذكاء الاصطناعي يفهم وثائقك بالصح — بالعربية.**

كي تعطي لوكيل ملف PDF ولا Word ولا جدول Excel ولا صورة صفحة ممسوحة، يوقعو زوج مشاكل: العربية اللي داخل تخرج معكوسة ومشوشة، وحتى كي تخرج نظيفة تكون مكتوبة بلغة رسمية صعيبة حتى واحد ما يشرحهالك. هذه المهارة (SKILL.md واحد) تعلّم أي وكيل يقرا الوثيقة، يصلّح العربية المكسورة بدل ما يعاودها، ومن بعد يشرحلك واش تقول الوثيقة بعربية واضحة وبسيطة (ولا بالدارجة)، يجاوب على أسئلتك عليها، ويلخّصها كي تطلب. الأرقام تبقى مضبوطة، واللي ما يقدرش يقراه يقولك ما قدرتش — ما يخمّنش أبداً.

## التركيب

```
npx skills add dagdog16-beep/arabic-doc-reader
```

*(مسودة — المستودع يتحط وقت النشر.)*

تخدم مع Claude Code وCodex وCursor وCopilot وGemini CLI وباقي منصات الوكلاء اللي تدعم المهارات.

## واش يبدّل

نفس الصفحة من فاتورة، كيما خرجت من الاستخراج — وكيما ترجع بهذه المهارة:

| مستخرجة (مكسورة) | مصلّحة ومشروحة |
|---|---|
| `يرهشلا غلبملا يلامجإ : رالود 250` | المبلغ الشهري الإجمالي: 250 دولار — «هذا هو المبلغ اللي لازم تخلصو كل شهر» |

أمثلة كاملة في [examples.md](examples.md). القواعد كاملة في [SKILL.md](SKILL.md).

## الخصوصية

وثيقتك تتقرا داخل محادثتك برك. هذه المهارة ما تخزّن والو، ما تبعث والو لأي بلاصة، وما تخلي والو بين المحادثات.

## تحتاج الأدوات الثقيلة؟

هذه المهارة تشرح وثيقة وحدة في كل مرة، داخل محادثة. للخدمة الثقيلة، نفس الصانع يدير:

- **مُصلِح النص العربي** — مجاني، يصلّح ملفات كاملة من العربية المعكوسة والمشوشة (استخراجات PDF وWord) دفعة وحدة: [GitHub](https://github.com/dagdog16-beep/arabic-text-fixer) · [Payhip](https://payhip.com/b/xcAmu)
- **المفرّغ** — يحوّل المحاضرات والاجتماعات وملفات الصوت والفيديو إلى نص عربي، 100% بلا إنترنت: [Payhip](https://payhip.com/b/0Y8UN)

من **Ali Ramdani — Dagdog Tools** (مونتريال) — أدوات صغيرة لمشاكل حقيقية، تعمل بلا إنترنت: [Gumroad](https://dagdog2.gumroad.com) · [Payhip](https://payhip.com/DagdogTools)

الترخيص: MIT.
