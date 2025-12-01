
# 📍 WhatsApp Shop Location Update & Sharing (HTML + CSS + JavaScript)

This project is a **WhatsApp-style login interface** that allows shop owners to quickly **enter their username, password, WhatsApp number, and new shop address**, and instantly **send the updated shop location to customers via WhatsApp**.

It does not use any backend — everything runs **fully client-side**.

---

## ✨ Features

✔ Modern WhatsApp-themed UI (dark mode design)
✔ Login input (demo-only, client-side validation)
✔ Enter WhatsApp phone number (international format)
✔ Enter new shop address
✔ Auto-generates WhatsApp message
✔ Opens WhatsApp Web (desktop) or WhatsApp App (mobile)
✔ Preview message before sending
✔ No database, no backend — pure HTML/CSS/JS
✔ Lightweight and mobile responsive
✔ Clean UI with animations and validation

---

## 🧠 How It Works

1. User fills:

   * Username
   * Password
   * WhatsApp number
   * New shop address

2. The app validates:

   * Username ≥ 3 characters
   * Password ≥ 6 characters
   * WhatsApp number = digits (6–15 length)
   * Address not empty

3. A message is generated:

```
Hello, this is <username>.
I am updating my shop location. New address:
<your address>

Sent on: <date & time>
```

4. The script redirects to:

```
https://wa.me/<number>?text=<encoded message>
```

5. WhatsApp opens with the **pre-filled message** ready to send.

---

## 🧩 Technologies Used

* **HTML5** (UI layout & components)
* **CSS3** (WhatsApp-inspired dark theme, gradients, responsive design)
* **Vanilla JavaScript**

  * Input validation
  * WhatsApp deep link generator
  * Message preview
  * Fake login check
* No frameworks
* No server required

---

## 📁 Folder Structure (Single File Project)

```
index.html
```

Contains:

* All HTML
* Embedded CSS (WhatsApp-style design)
* Embedded JavaScript logic

---

## 📸 UI Overview

* WhatsApp Dark-Themed Login Panel
* Input groups with green focus borders
* Buttons: Primary, Ghost, Reset
* Right side “How it works” section
* Error messages + validation UI

---

## 🚀 Usage

1. Download or clone repo
2. Open `index.html` in any browser
3. Enter your details
4. Click **Login & Send on WhatsApp**
5. WhatsApp Web/App opens with your message

---

## 📝 Customization Options

You can easily modify:

* Message text → in `buildMessage()`
* UI colors → CSS `:root` variables
* Authentication → replace `fakeLogin()` with backend login
* Phone number format
* Add map integration (optional future update)




