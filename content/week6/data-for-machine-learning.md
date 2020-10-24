---
title: "داده برای یادگیری ماشین"
date: 2020-10-19T22:37:58+03:30
draft: false
weight: 110
---

چه مقدار داده را باید آموزش دهیم؟
در موارد مشخص، یک **الگوریتم کم کیفیت** با داده بیشتر، میتواند عملکرد بهتری نسبت به یک **الگوریتم با کیفیت** و داده کمتر داشته باشد.

ما باید ویژگی‌هایی را انتخاب کنیم تا اطلاعات کافی داشته باشیم. یک آزمون مفید به این صورت است که: با توجه به ورودی x، آیا یک متخصص انسانی می‌تواند با اطمینان y را پیش بینی کند؟

**منطق داده‌های بزرگ**: اگر یک الگوریتم با بایاس کم داشته باشیم (ویژگی‌های زیاد یا واحدهای پنهان یک تابع بسیار پیچیده می‌سازد)، پس هرچه مجموعه آموزشی بزرگتر باشد، overfitting کمتری خواهیم داشت (و الگوریتم روی مجموعه آزمون دقیق‌تر خواهد بود).