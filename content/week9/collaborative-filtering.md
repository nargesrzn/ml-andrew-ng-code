---
title: "فیلترینگ مشارکتی"
date: 2020-11-05T22:48:50+03:30
draft: false
weight: 110
---

پیدا کردن ویژگی‌هایی مانند "تعداد صحنه‌های عاشقانه" یا "تعداد صحنه‌های اکشن" در فیلم می‌‌تواند بسیار سخت باشد. برای پی بردن به این مسئله، می‌توان از "ویژگی یاب‌ها" استفاده کرد.

می‌توانیم به کاربران اجازه دهیم به ما نشان دهند که چقدر ژانرهای مختلف را دوست دارند که بلافاصله بردار پارامتر را برای ما فراهم می‌کند.

برای پی بردن به ویژگی‌ها از پارامترهای موجود، از تابع خطای مجذور با منظم‌سازی بر روی تمامی کاربران استفاده می‌کنیم:

$$min_{x ^{(1)}, ...,x ^{(n_{m })}} = \frac{1}{2}\sum_{i=1}^{n_{m }}\sum_{i:r(i,j)=1}^{}((\theta ^{(j)})^{T}(x^{(i)}) - y^{(i,j)})^{2} + \frac{\lambda }{2}\sum_{i=1}^{n_{m }}\sum_{k=1}^{n}(x _{k}^{(i)})^{2}$$

همچنین می‌توانید مقادیر تتا را به صورت **تصادفی حدس بزنید** تا به صورت متوالی ویژگی‌ها را حدس بزنید. در واقع شما به مجموعه مناسبی از ویژگی‌ها همگرا خواهید شد.