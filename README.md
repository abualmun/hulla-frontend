# 📖 Hulla (حُـلَّـة)

🌟 *A modern solution to organize and track Quran memorization for students and teachers.*

---

## ✨ About The Project

Keeping track of Quran memorization progress in a college environment can be overwhelming 📚. Traditional methods like papers and spreadsheets are inefficient and error-prone 🧾❌. **Hulla** was created to solve this challenge by offering a digital, user-friendly experience.

👨‍🏫 **Teachers** can:

* View student history
* Filter by date 🗓️
* Add/edit/delete records

🧑‍🎓 **Students** can:

* Track their own progress
* Stay motivated and organized 💪

This app bridges the gap between spiritual growth and smart technology 💡🕌.

---

## 🚀 Features

✅ Role-based views (Students 👨‍🎓 / Teachers 👩‍🏫)
✅ Student selection dropdown 📋
✅ Memorization record logging (Surah, Ayahs, Grade) 📖
✅ Date range filtering for reports 🗂️
✅ Full CRUD for memorization records ✍️
✅ Cross-platform: Android 🤖, Web 🌐, Linux 🐧

---

## 🛠️ Built With

* 🧩 **Flutter** – UI toolkit for multi-platform apps
* 🧠 **Dart** – The language behind Flutter
* 🔌 **http** – API integration
* 📦 **flutter\_bloc** – State management
* 🕰️ **intl** – Date formatting

---

## 🏁 Getting Started

### 📋 Prerequisites

* Flutter SDK (stable channel, version ≥ 2.15.1)
* IDE like VS Code or Android Studio

### 🔧 Installation & Setup

1. **Clone the repository**

```bash
git clone https://github.com/[YOUR_GITHUB_USERNAME]/abualmun-hulla-frontend.git
cd abualmun-hulla-frontend
```

2. **Install dependencies**

```bash
flutter pub get
```

3. **Configure Backend API**

Edit:

* `lib/model/user_model.dart`
* `lib/model/records_model.dart`

Update the API endpoints in `Uri.parse('')` with your actual backend URL.

```dart
// Example
final response = await http.Client().post(
  Uri.parse('https://your-api-endpoint.com/login'),
);
```

4. **Run the app**

```bash
flutter run
```

Use your IDE to run it on your device of choice: Android, Web, or Linux.

---

## 🗄️ Backend API Requirements

To work properly, the backend must implement:

* `POST /login` – Authenticate users
* `POST /records/fetch` – Fetch memorization records
* `POST /records/add` – Add a new record
* `POST /records/edit` – Modify an existing record
* `POST /records/delete` – Remove a record by ID

---

## 📂 Project Structure

```
lib/
├── main.dart               # Entry point
├── model/
│   ├── records_model.dart  # Record model & API
│   └── user_model.dart     # User model & API
└── view/
    └── login_screen.dart   # Login UI
```

---

## 🤝 Contributing

Contributions are what make the open-source community amazing! 🫶

💡 Got an idea?
🔧 Found a bug?
✨ Want to add features?

Fork the repo, create your feature branch, and open a pull request:

```bash
git checkout -b feature/AmazingFeature
git commit -m 'Add some AmazingFeature'
git push origin feature/AmazingFeature
```

We'd love to see your contributions! 🙌

---
