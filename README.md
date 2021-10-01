# ArraysArrays
في الكوتلن نستطيع إنشاء مصفوفات Arrays عن طريق المكتبة الموجودة في اللغة 

arrayOf()
المثال التالي لإنشاء مصفوفة أرقام Int

val numbers = arrayOf(1, 2, 3, 4, 5, 6)
و مرة أخرى خاصية الـ Type inference في الكوتلن تستنتج نوع المصفوفة من خلال القيم الخاصة بها. 

و للوصول إلى عناصر المصفوفة هناك طريقتين 
الطريقة الأولى:
عن طريق معرفة الفهرس index للعنصر كالتالي:

numbers[2] = 30
هنا تم تغيير القيمة ٣ إلى ٣٠ عن طريق الindex , و نلاحظ أن الفهرسة للمصفوفات تبدأ من الصفر لأول عنصر.

الطريقة الثانية:
عن طريق معرفة الفهرس index للعنصر باستخدام الدوال get و set.

فالمثال التالي يتم استخدام الدالة get  للحصول على قيمة العنصر الرابع في المصفوفة لغرض تخزينه في متغير آخر مثلا, فالدالة get تستخدم لاسترجاع قيمة العناصر داخل المصفوفة :

var num = numbers.get(3)
و نستخدم الدالة set مع المصفوفات لتغيير القيم إلى قيم اخرى, المثال التالي نستطيع تغيير العنصر السادس إلى القيمة ٦٠٠ بدلا من ٦ كالتالي:

numbers.set(5, 600)
لمعرفة حجم المصفوفة
نستخدم الخاصية size لمعرفة الحجم و تعود لنا بقيمة integer, فالسطر التالي يطبع لنا الرقم ٦ و هي عدد عناصر المصفوفة:

println(numbers.size)
