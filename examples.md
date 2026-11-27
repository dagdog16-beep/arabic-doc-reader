# Examples — أمثلة

Three documents, the way this skill handles them: repair first, explain in plain words, never invent.

---

## 1) A PDF whose Arabic extracted reversed — فاتورة PDF خرجت معكوسة

**What the extraction gave the agent:**

```
ةحفصلا 1 نم 1
يرهشلا غلبملا يلامجإ : رالود 250
يئاهنلا دعوملا : سطسغأ 15
```

**What the skill answers:**

> النص وصلني معكوس — صلّحتو قبل ما نشرح. هذه فاتورة من صفحة وحدة، وهذا واش تقول:
>
> - **المبلغ الشهري الإجمالي: 250 دولار** — هذا هو المبلغ اللي لازم يتخلص هاذ الشهر.
> - **الموعد النهائي: 15 أغسطس** — بعد هذا التاريخ يقدر يتزاد عليك مبلغ التأخير.
>
> باختصار: عندك 250 دولار تخلصها قبل 15 أغسطس.

The repair: the extracted text is restored to its real order («المبلغ الشهري الإجمالي»، «الموعد النهائي») — the reversed text is never repeated to the user as if it were normal, and the numbers stay exactly where the document put them.

---

## 2) An Excel sheet — جدول Excel والمجموع

**What the sheet contains:** a small shop's monthly expenses — rows for الإيجار (rent) 900، الكهرباء (electricity) 120، الماء (water) 45، البضاعة (stock) 1,300 — and an empty total row at the bottom.

**What the skill answers:**

> هذا الجدول هو مصاريف المحل تاع هاذ الشهر، فيه 4 حوايج:
>
> - الإيجار: 900
> - الكهرباء: 120
> - الماء: 45
> - البضاعة: 1,300
>
> خلية المجموع في الجدول خاوية — الجدول نفسو ما عطاش مجموع. جمعتهم أنا: **900 + 120 + 45 + 1,300 = 2,365**. هذا المجموع من حسابي أنا، مش مكتوب في الجدول — راجع الأرقام الأربعة بنفسك باش تتأكد.

The rule at work: numbers copied exactly, and a total the agent calculated itself is labelled as its own calculation — never presented as something the document said.

---

## 3) A scanned page, partly unreadable — صفحة ممسوحة، جزء منها ما يتقراش

**What the scan looks like:** a photographed official letter. The top half is sharp; the bottom half is blurry, and a round stamp covers part of the last lines.

**What the skill answers:**

> قريت الصفحة. النصف اللي الفوق واضح، وهذا واش يقول: الرسالة من البلدية، تخبرك بلي ملفك وصل، ورقم الملف هو **2026-1843**.
>
> **بصراحة: النصف اللي التحت ما قدرتش نقراه.** التصويرة ضبابية ثما، وكاين ختم دائري مغطي جزء من السطور الأخيرة — والتاريخ اللي في الآخر ما بانليش كامل، ما نقدرش نخمّنو.
>
> باش نكملك الشرح: صوّر الصفحة مرة أخرى من قريب وبلا ما يتحرك الهاتف، وحاول الختم ما يغطيش السطور — ولا ابعث الصفحة الثانية إذا كاينة.

The rule at work: what was readable is explained, what was not is named plainly — part, reason, and what would fix it. A date hidden under a stamp is never invented.
