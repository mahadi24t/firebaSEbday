

```markdown
# 🎉 Birthday App

A simple and stylish web app for saving birthdays to Firebase Realtime Database. Just type a name and date—like `Walt Disney: 05.12.1901`—and click **Add**!

![Birthday GIF](assets/happybirthday.gif)

---

## ✨ Features

- Clean, responsive interface with custom Google Fonts
- Input field for birthday entries
- Realtime Firebase backend using CDN modules
- Lightweight and beginner-friendly frontend—no build tools required

---

## 🚀 Getting Started

### 1. Clone this Repository
```bash
git clone https://github.com/your-username/birthday-app.git
cd birthday-app
```

### 2. Launch a Local Server
To avoid browser CORS issues with modules, use Live Server (VS Code) or run:
```bash
npx serve
```

### 3. Firebase Setup
- Create a Firebase project at [firebase.google.com](https://firebase.google.com/)
- Enable **Realtime Database**
- Replace `firebaseConfig` in `index.js` with your own:
```js
const firebaseConfig = {
  databaseURL: "https://your-project-id.firebaseio.com"
};
```

### 4. Development Rules (Temporary)
Go to Realtime Database → Rules and set:
```json
{
  "rules": {
    ".read": true,
    ".write": true
  }
}
```

> ⚠️ These rules allow public read/write access. Use for testing only!

---

## 🗂 Project Structure

```
/
├── index.html        # App layout
├── index.css         # Styling
├── index.js          # Logic + Firebase connection
└── assets/
    └── happybirthday.gif
```

---

## 🌟 Future Ideas

- Display saved birthday list
- Edit/delete functionality
- Form validation and feedback
- Authentication with Firebase

---

## 🎨 Credits

- Font: [Josefin Sans](https://fonts.google.com/specimen/Josefin+Sans)
- GIF: Your own `assets/happybirthday.gif`

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
```

You’re all set! Let me know if you’d like help deploying to GitHub Pages or Firebase Hosting next.
