---
title: "الگوریتم فیلترینگ مشارکتی"
date: 2020-11-05T22:46:23+03:30
draft: false
weight: 120
---

برای سرعت بخشیدن به کارها، می‌توانیم ویژگی‌ها و پارامترها را به صورت همزمان به حداقل برسانیم:

$$
J(x,\theta ) = \frac{1}{2}\sum_{(i,j):r(i,j)=1}^{}((\theta ^{(j)})^{T}(x^{(i)}) - y^{(i,j)})^{2} + \frac{\lambda }{2}\sum_{i=1}^{n_{m }}\sum_{k=1}^{n}(x_{k}^{(i)})^{2} + \frac{\lambda }{2}\sum_{j=1}^{n_{u }}\sum_{k=1}^{n}(\theta _{k}^{(j)})^{2}
$$

این روش ممکن است پیچیده به نظر بیاید اما فقط تابع هزینه برای تتا و تابع هزینه x را ترکیب کردیم.

چون الگوریتم می‌تواند این موارد را خودش یاد بگیرد، واحدهای بایاس که در آن‌ها $x_{0} =1$ باشد، حذف شده‌اند، از این رو $x \in \mathbb{R}^{n}$ و $\theta \in \mathbb{R}^{n}$.

مراحل الگوریتم به صورت زیر خواهند بود:

1. $( x^{(i)}, ..., x^{(n_{m})}, \theta ^{(1)}, ..., \theta ^{(n_{u })})$ را به مقادیر تصادفی کوچک، مقداردهی کنید. این کار به منظور از بین بردن تقارن انجام می‌شود و تضمین می‌کند که الگوریتم ویژگی‌های $x^{(i)}, ..., x^{(n_{m})}$ را یاد بگیرد که با هم متفاوت هستند.

2. با استفاده از گرادیان کاهشی (یا یک الگوریتم بهینه‌سازی پیشرفته) $J( x^{(i)}, ..., x^{(n_{m})}, \theta ^{(1)}, ..., \theta ^{(n_{u })})$ را به حداقل برسانید. بطور مثال برای هر 

$j=1,...,n_{u}, i=1,...,n_{m}:x_{k}^{(i)}:=x_{k}^{(i)} - \alpha (\sum_{j:r(i,j)=1}^{}((\theta ^{(j)})^{T}x^{(i)} - y^{(i,j)})\theta_{k}^{(j)} + \lambda x_{k}^{(i)})$

$\theta_{k}^{(j)}:= \theta_{k}^{(j)} - \alpha (\sum_{i:r(i,j)=1}^{}((\theta ^{(j)})^{T}x^{(i)} - y^{(i,j)})x_{k}^{(i)} + \lambda \theta _{k}^{(j)})$

3. برای یک کاربر با پارامترهای $\theta$ و یک فیلم با ویژگی‌های (یادگرفته شده) x، رتبه‌بندی ستاره‌ای $\theta^{T}x$ را پیش‌ بینی کنید.