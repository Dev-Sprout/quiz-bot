# 📚 Quiz Bot – Telegram Viktorina Bot

Telegram bot orqali foydalanuvchilar o‘z testlarini yaratadi, guruhda ulashadi va test yakunida natijalarni ko‘radi.

---

## ⚙️ Funktsiyalar

- Foydalanuvchi o‘zi test yozadi va botga yuboradi
- Bot testni bazaga yozadi va link yaratadi
- Linkni guruhga yuborish mumkin
- Guruhdagi foydalanuvchilar testga qo‘shiladi
- Test avtomatik boshlanadi
- Har bir savol navbatma-navbat chiqadi
- Har bir ishtirokchi natijasini ko‘radi
- Guruhda umumiy reyting chiqariladi

---

## 📌 Ishlash Tartibi

1. **/start** – Botni boshlash
2. **Test yuborish** – Maxsus formatda savollar yuboriladi:

    ```
    Savol: Yer quyosh atrofida qancha vaqtda aylanishni tugatadi?
    A) 24 soat
    B) 1 oy
    C) 365 kun
    D) 7 kun
    Javob: C
    ```

3. **Bot formatni tekshiradi** va testga ID beradi
4. **Test linki** beriladi:
    ```
    https://t.me/quiz_bot?start=test123
    ```
5. **Guruhda test boshlanishi uchun foydalanuvchilar “✅ Tayyorman” tugmasini bosadi**
6. **Test boshlanadi va har savolga vaqt belgilanadi**
7. **Test tugagach, natijalar ko‘rsatiladi**

---

## 💾 Texnologiyalar

| Qism               | Texnologiya         |
|--------------------|---------------------|
| Telegram bot       | Python + aiogram    |
| Ma’lumotlar bazasi | PostgreSQL          |
| Hosting            | Railway / Render    |
| Fayllar            | Pandas, PDFKit      |

---

---

## 📊 Foydalanish senariylari

### 1. Test yaratish

1. Foydalanuvchi `/create_test` buyrug‘i orqali yangi test yaratadi.
2. Savollarni quyidagi formatda yuboradi:
    ```
        Savol matni?
        A) Variant A
        B) Variant B
        C) Variant C
        D) Variant D
        Javob: B
    ```
3. Bot ushbu savollarni tekshiradi va saqlaydi.
4. Testga ulanish havolasi yaratiladi va foydalanuvchiga yuboriladi.

---

### 2. Guruhga testni ulashish

- Foydalanuvchi olgan test havolasini guruhga yuboradi.
- Guruh a’zolari “✅ Ishtirok etaman” tugmasini bosish orqali qatnashishga rozi bo‘ladi.
- Yetarli son ishtirokchi to‘plangach, test avtomatik boshlanadi.

---

### 3. Testni ishlash

- Har bir ishtirokchiga savollar navbatma-navbat yuboriladi.
- Har bir savol uchun vaqt cheklovi (masalan: 30 soniya) bo‘lishi mumkin.
- Foydalanuvchi javob variantlaridan birini tanlaydi.

---

### 4. Natijalarni ko‘rish

- Test tugagach, umumiy natijalar guruhda e’lon qilinadi.
- Har bir ishtirokchi o‘zining yakuniy natijasini shaxsiy xabarda oladi:
  - To‘g‘ri javoblar soni
  - Foiz hisobidagi natija
  - Qaysi savollarda xato qilgani

---

## 🧪 Test holati

| Holat          | Status           |
|----------------|------------------|
| Test yaratish  | ✅ Ishlaydi       |
| Savollar saqlash | ✅ Ishlaydi     |
| Test ulashish  | ✅ Ishlaydi       |
| Viktorina boshlanishi | 🔄 Rejalashtirilmoqda |
| Natijalarni ko‘rish | 🔄 Rejalashtirilmoqda |

---

## 🔐 Xavfsizlik

- Har bir testga unikal ID biriktiriladi
- Ma’lumotlar PostgreSQL bazasida saqlanadi
- Faqat test yaratuvchisi o‘z testlarini ko‘ra oladi

---


## 👨‍💻 Muallif

- Mansurbek – [Telegram](https://t.me/madirimov_411)

---
