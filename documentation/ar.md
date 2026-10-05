<!-- ELUCENIA technical documentation · fib-4 · ar · no clinical/professional/rights approval -->

# FIB-4 (تليف الكبد)

[الشروط والمصادر والأذونات](https://elucenia.org/ar/tools/fib-4)

## كيفية الاستخدام

استخدم الأداة في البوابة أو افتح index.html عبر خادم HTTP محلي. اختر اللغة، وأكمل الحقول، ثم أجرِ الحساب.

## المدخلات والوحدات

### العمر

`idade`

سنوات · النطاق: ١٨–١٠٠

### AST

`ast`

U/L · النطاق: ١–٥٠٠٠

### ALT

`alt`

U/L · النطاق: ١–٥٠٠٠

### الصفائح الدموية

`plq`

× 10³/mm³ · النطاق: ٥–١٥٠٠

### السياق

`etio`

- `masld` — تشحّم الكبد (MASLD/NAFLD)
- `viral` — التهاب الكبد C أو HIV/HCV

## إصدار الطريقة

FIB-4/Sterling 2006؛ عتبات HCV/HIV 1.45/3.25 مقابل MASLD 1.3/2.67 ومن عمر ≥65 سنة 2.0

## المعادلة الموثقة

FIB-4 = (العمر × AST) ÷ (الصفائح \[10⁹/L\] × √ALT).

MASLD: \< 1.30 يستبعد التليّف المتقدّم (\< 2.0 من عمر 65)؛ \> 2.67 يشير إلى تليّف متقدّم. التهاب الكبد C/HIV: \< 1.45 و\> 3.25.

## الحدود والفئة السكانية

طُورت FIB-4 من Sterling لعام 2006 لدى مرضى مصابين بعدوى HIV/HCV المشتركة، مع تقييم الحدين \<1,45 و\>3,25 مقابل درجات تليف Ishak ‏4–6. تستخدم المعادلة العمر بالسنوات وAST وALT بوحدة U/L والصفائح بوحدة 10^9/L. لا يمكن استبدال هذه الحدود والفئة الأصلية تلقائيًا بمعايير MASLD أو التعديلات حسب العمر؛ فتلك الصيغ تتطلب مصادر خاصة بها.

## المراجع

- [Sterling RK et al. Development of a simple noninvasive index to predict significant fibrosis in patients with HIV/HCV coinfection. Hepatology, 2006.](https://doi.org/10.1002/hep.21178)

- [Shah AG et al. Comparison of noninvasive markers of fibrosis in patients with nonalcoholic fatty liver disease. Clin Gastroenterol Hepatol, 2009.](https://doi.org/10.1016/j.cgh.2009.05.033)

- [McPherson S et al. Age as a confounding factor for the accurate non-invasive diagnosis of advanced NAFLD fibrosis. Am J Gastroenterol, 2017.](https://doi.org/10.1038/ajg.2016.453)

- [Rinella ME et al. AASLD Practice Guidance on the clinical assessment and management of nonalcoholic fatty liver disease. Hepatology, 2023.](https://doi.org/10.1097/HEP.0000000000000323)

## إعادة إجراء الاختبارات التقنية

شغّل node test.cjs في المجلد الجذري لهذا المستودع لتكرار الحالات الاصطناعية المسجلة. تُحفظ المدخلات والنتائج المتوقعة وحدود التفاوت الأصلية. لا تُعدّ الاختبارات التقنية تحققًا سريريًا.

```sh
node test.cjs
```

يحتوي tool.json على المصادر والإصدار ونطاق المراجعة. يحتفظ examples.json بالمدخلات والنتائج المتوقعة للحالات الاصطناعية؛ ويسجل results.json النتائج التي تم الحصول عليها.

[السجل والمراجع](../tool.json) · [شيفرة JavaScript](../calculator.js) · [حالات مرجعية](../examples.json) · [results.json](../results.json)

## المراجعة وشروط الاستخدام

لم تُجرَ مراجعة سريرية مستقلة.

هذه الواجهة ترجمة أعدّها مؤلفوها، وليست إصدارًا رسميًا أو معتمدًا. لم تُجرَ مراجعة سريرية مستقلة أو مراجعة لغوية مهنية، ولم تُستكمل الموافقة على حقوق استخدام الأدوات.

نتيجة المعادلة أو التصنيف. يعتمد التفسير والتصرف ومدى الانطباق على التقييم المهني والمصدر المحدد.

## الترخيص ونسبة العمل إلى أصحابه

ينطبق Apache-2.0 على كود ELUCENIA فقط. تبقى حقوق الأدوات والمنشورات والترجمات والبيانات لأصحابها المعنيين. احتفظ بملفّي LICENSE وNOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
