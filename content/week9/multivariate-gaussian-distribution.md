---
title: "توزیع گاوسی چند متغیره(اختیاری)"
date: 2020-10-30T20:06:14+03:30
draft: false
weight: 70
---

توزیع گاوسی چند متغیره در واقع تعمیم تشخیص ناهنجاری است و ممکن است (یا ممکن نیست) ناهنجاری‌های بیشتری را پیدا کند.

به جای مدل‌ سازی جداگانه $p(x_{1})$، $p(x_{2})$، ...  ما $p(x)$ را در یک مرحله مدل سازی می‌کنیم. پارامترهای ما $\mu \in \mathbb{R}^{n}$ و $\Sigma  \in \mathbb{R}^{n \times n}$ خواهند بود.


$p(x; \mu , \Sigma ) = \frac{1}{(2\pi )^{\frac{n}{2}}\left | \Sigma  \right |^{\frac{1}{2}}}exp(-\frac{1}{2}(x - \mu )^{T}\Sigma ^{-1}(x-\mu ))$

یک نتیجه مهم این است که می‌توانیم خطوط مستطیلی گاوسی را مدل کنیم که این امکان را به ما می‌دهد تا داده‌هایی را متناسب کنیم که ممکن است در خطوط دایره‌ای طبیعی جای نگیرند.

متغیر $\Sigma$ شکل، پهنا و جهت خطوط را تغییر می‌دهد. تغییر $\mu$ مرکز توزیع را جابجا خواهد کرد.


همچنین لینک زیر را مطالعه کنید:
- [توزیع گاوسی چندمتغیره](http://cs229.stanford.edu/section/gaussians.pdf) Chuong B. Do, October 10, 2008.