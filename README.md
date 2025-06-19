<div align="center">
  <h1>🎴 3D Card Component</h1>
  <p>Interactive 3D flip card with image and video support</p>
</div>

---

## 📌 Overview

Bu loyiha foydalanuvchi ustiga hover qilganda 3D tarzda aylanuvchi interaktiv karta yaratish imkonini beradi. Karta ichida siz rasm (img) yoki video (mp4, webm) joylashtirishingiz mumkin. **Hover effekti**, **backface visibility**, **transform** funksiyalaridan foydalanilgan.

---

## ✨ Xususiyatlar

- 🔁 3D aylanish (Flip) animatsiyasi
- 🖼 Rasm joylash imkoniyati (`img`)
- 🎥 Video o‘rnatish imkoniyati (`video`)
- 📱 Responsive dizayn
- 💡 Sof HTML/CSS va JavaScript (kutubxonasiz)

---

## 📂 Loyihaning tuzilishi

```
📁 3d-card-project/
├── 📄 index.html
├── 📄 style.css
├── 📁 assets/
│   ├── 📷 image.jpg
│   └── 🎞 video.mp4
└── 📄 README.md
```

---

## 🛠 O‘rnatish

```bash
# Git orqali yuklab oling
git clone https://github.com/yourusername/3d-card-project.git

# Papkaga kiring
cd 3d-card-project

# Brauzerda index.html faylni oching
```

---

## 🧩 HTML namunasi

```html
<div class="card">
  <div class="card-inner">
    <div class="card-front">
      <img src="./assets/image.jpg" alt="Card Front Image" />
    </div>
    <div class="card-back">
      <video src="./assets/video.mp4" autoplay muted loop></video>
    </div>
  </div>
</div>
```

---

## 🎨 CSS Asosiysi (`style.css`)

```css
.card {
  width: 300px;
  height: 200px;
  perspective: 1000px;
}

.card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  transition: transform 1s;
  transform-style: preserve-3d;
}

.card:hover .card-inner {
  transform: rotateY(180deg);
}

.card-front, .card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
  border-radius: 12px;
  overflow: hidden;
}

.card-front img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.card-back {
  transform: rotateY(180deg);
  background-color: #000;
}

.card-back video {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```

---

## 🖼 Rasm joylash

1. `assets/` papkasiga rasm (`.jpg`, `.png`, `.webp`) joylang.
2. HTML’da quyidagicha yozing:

```html
<img src="./assets/image.jpg" alt="My 3D Image" />
```

---

## 🎥 Video joylash

1. `assets/` papkasiga video (`.mp4`, `.webm`) faylni saqlang.
2. HTML’da:

```html
<video src="./assets/video.mp4" autoplay muted loop></video>
```

✅ `autoplay`, `muted`, `loop` atributlari videoni avtomatik va qayta-qayta o‘ynatish uchun kerak.

---

## 🧪 Namuna rasm va video

| Old taraf (Rasm) | Orqa taraf (Video) |
|------------------|--------------------|
| ![Card Front](./assets/sample-front.jpg) | ![Card Back](./assets/sample-back.gif) |

> Eslatma: GitHub’da video preview to‘liq ko‘rinmaydi, lekin loyihangizda `.mp4` to‘liq o‘ynaydi.

---

## 📬 Muallif bilan bog‘lanish

- **Ism:** ASLWEX King
- **Telegram:** [@asldeveloper](https://t.me/asldeveloper)
- **GitHub:** [AslDeveloper07](https://github.com/AslDeveloper07)

---

## 📜 Litsenziya

Ushbu loyiha **MIT License** asosida tarqatiladi. Istagancha foydalanishingiz mumkin.

---

> 3D karta loyihasi ta'lim, portfolio, e-commerce yoki video prewievlar uchun juda foydali.
