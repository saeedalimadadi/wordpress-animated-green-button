# 🟢 WordPress Animated Green Button

A clean, lightweight, and responsive **HTML + CSS button** built for WordPress posts and any HTML page.  
It features a **white background**, **black text**, **#03fc62 green border**, and a **center-fill hover animation** that smoothly changes the background and text color.

---

## 🌟 Features
- 🧩 Works directly inside WordPress posts or Elementor HTML widgets  
- 🎨 Clean and minimal design  
- ⚡ Fast and lightweight (pure CSS, no JS)  
- 🟢 Smooth hover animation (fill from center)  
- 💬 Fully customizable (color, size, radius, text)  
- 📱 Responsive and theme-friendly  

---


##Replace:

🔗 href → with your product link

🏷 <span>View Product</span> → with your button text

##🧱 Demo

You can view a live demo by opening index.html in your browser.

⚙️ Customization
Property	Description	Example
#03fc62	Border & fill color	Change to your brand color
border-radius	Button shape	8px (square) or 50px (pill)
padding	Button size	10px 24px
font-size	Text size	18px

---

📜 License

This project is licensed under the MIT License — free for commercial and personal use.
See LICENSE
 for details.
---
🇮🇷 توضیحات فارسی

این پروژه یک دکمه‌ی HTML + CSS سبک و مدرن برای وردپرس است
که هنگام هاور شدن، رنگ سبز از مرکز پر شده و نوشته سفید می‌شود.
به‌صورت مستقیم داخل پست‌های وردپرس یا ابزارک HTML المنتور قابل استفاده است.

✳ ویژگی‌ها:

دکمه سفید با متن مشکی و بوردر سبز

افکت پر شدن رنگ از مرکز هنگام هاور

بدون نیاز به جاوااسکریپت

قابل شخصی‌سازی از نظر رنگ، اندازه، و فونت

💡 روش استفاده:

کافی است کد زیر را در هر بخش از محتوای پست خود قرار دهید.
فقط لینک و متن دکمه را تغییر دهید.

Developed by: [Saeed Alimadadi + ChatGPT AI]

---

## 🚀 Quick Usage

Paste this snippet anywhere inside your WordPress post (Classic Editor or Block Editor):

```html
<a href="https://yourwebsite.com/product-page" class="magic-button"><span>View Product</span></a>

<style>
.magic-button {
  display: inline-block;
  padding: 12px 28px;
  font-size: 16px;
  font-weight: 600;
  color: black;
  background-color: white;
  border: 2px solid #03fc62;
  border-radius: 50px;
  cursor: pointer;
  position: relative;
  overflow: hidden;
  text-decoration: none;
  transition: color 0.4s ease;
}
.magic-button::before {
  content: "";
  position: absolute;
  top: 0;
  left: 50%;
  transform: translateX(-50%) scaleX(0);
  width: 100%;
  height: 100%;
  background-color: #03fc62;
  transition: transform 0.4s ease;
  transform-origin: center;
  z-index: 0;
}
.magic-button:hover::before {
  transform: translateX(-50%) scaleX(1);
}
.magic-button span {
  position: relative;
  z-index: 1;
  transition: color 0.4s ease;
}
.magic-button:hover span {
  color: white;
}
</style>
