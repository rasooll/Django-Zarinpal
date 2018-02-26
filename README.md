# Django-Zarinpal
Sample Django ZarinPal WebGate with SOAP--By Parsae @ SAMAR Web Academy

<h1 dir="rtl">«بسم الله الرحمن الرحیم»</h1>
<img src="https://raw.githubusercontent.com/aparsaee/Django-Zarinpal/master/zarinpal-logo.png">
<p dir="rtl">با سلام و احترام خدمت شما دوستان بزرگوار</p>

<p dir="rtl">برای استفاده از درگاه پرداخت زرین پال به کمک فریمورک جانگو میتوانید از نمونه کد موجود در این پروژه استفاده کنید.این پروژه به زبان پایتون نوشته شده است</p>

<h1 dir="rtl">پیشنیازهای Soap</h1>
<p dir="rtl">
برای نصب ماژول‌های مربوطه می‌توانید از دستورات زیر استفاده نمایید:
</p>
<pre><code># pip install client</code></pre>
<pre><code># pip install suds</code></pre>

<h1 dir="rtl">راهنما</h1>

<p dir="rtl">در این پروژه فرض میکنیم که میخواهیم با زدن یک دکمه در یکی از صفحات سایت شما به صفحه اولیه پرداخت زرین پال هدایت شویم.بنابراین باید تعیین کرده باشید که با زدن آن دکمه آدرس زیر فراخوانی شود
</p>

<pre><code>urls.py >>> url(r'^request/$', views.send_request, name='request')</code></pre>
<p dir="rtl">آدرس بالا به جانگو فرمان میدهد که از مسیر زیر تابع زیر فراخوانی شود</p>

<pre><code>views.py >>> send_request </code></pre>
<p dir="rtl">از این پس بقیه پردازش ها در سمت وب سرویس زرین پال انجام میشود</p>

<p dir="rtl">وب سرویس زرین پال مقادیری از جمله مرچنت کد، مبلغ و توضیحات را از شما میگیرد و در صورت صحت اطلاعات، شما را به سمت درگاه پرداخت بانک هدایت میکند.ار این پس پرداخت شما موفقیت آمیز باشد یا نباشد یا هر حالت دیگر،پردازش جانگو وارد تابع زیر در مسیر زیر میشود</p>

<pre><code>views.py >>> verify </code></pre>
<p dir="rtl">در تابع فوق حالات مختلف موفقیت یا عدم موفقیت پرداخت شما تعریف شده است که شما میتوانید به دلخواه خود خروجی آن را تغییر دهید</p>

<p dir="rtl">برای کسب اطلاعات بیشتر میتوانید به مستندات فنی اتصال به درگاه پرداخت زرین پال و فیلم های آموزشی سایت زرین پال در آپارات مراجعه فرمایید</p>


<p dir="rtl">موفق و پیروز باشید</p>

<p dir="rtl">پارسائی
</p>
