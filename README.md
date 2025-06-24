Hulla (حُـلَّـة) 📖

![alt text](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)


![alt text](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)


![alt text](https://img.shields.io/badge/platform-android%20%7C%20web%20%7C%20linux-lightgrey.svg?style=for-the-badge)

Hulla is a dedicated application built with Flutter, designed to help college students and their teachers organize and track the process of Quran memorization. It provides a simple and effective platform for managing records, monitoring progress, and facilitating communication between students and their mentors.

✨ About The Project

In our college, keeping track of Quran memorization progress between many students and teachers can be challenging. Manually recording on paper or in spreadsheets is inefficient and prone to errors. Hulla aims to solve this by providing a digital solution.

Teachers can easily view the memorization history of any student, filter records by date, and manage entries, while students have a clear view of their own progress. This project serves as a practical tool for our community, simplifying the administrative side of this blessed journey.

Screenshots

(You can add screenshots of your app here to make the README more engaging. Below are placeholders.)

Login Screen	Main Dashboard (Teacher's View)
[Image of Login Screen]	[Image of Main Dashboard]
🚀 Features

User Roles: Separate experiences for students and teachers/administrators.

Student Selection: Teachers can select a student from a dropdown to view their specific records.

Progress Tracking: Log new memorization records, including Sura, Ayah range, and grade.

Date Filtering: Use a date range picker to generate reports for a specific period.

CRUD Operations: Teachers can add, edit, and delete memorization records.

Cross-Platform: Built with Flutter, it's ready to be deployed on Android, Web, and Linux.

🛠️ Built With

This project is built using the following technologies:

Flutter - The UI toolkit for building natively compiled applications.

Dart - The programming language for Flutter.

http - For making API calls to the backend.

flutter_bloc - For state management.

intl - For date formatting.

🏁 Getting Started

To get a local copy up and running, follow these simple steps.

Prerequisites

Make sure you have the Flutter SDK installed on your machine (Stable channel, version >= 2.15.1).

A code editor like VS Code or Android Studio.

Installation & Setup

Clone the repository

Generated sh
git clone https://github.com/[YOUR_GITHUB_USERNAME]/abualmun-hulla-frontend.git


Navigate to the project directory

Generated sh
cd abualmun-hulla-frontend
IGNORE_WHEN_COPYING_START
content_copy
download
Use code with caution.
Sh
IGNORE_WHEN_COPYING_END

Install dependencies

Generated sh
flutter pub get
IGNORE_WHEN_COPYING_START
content_copy
download
Use code with caution.
Sh
IGNORE_WHEN_COPYING_END

Configure Backend API
This frontend application requires a backend to function. You will need to update the API endpoint URLs in the model files.

Open lib/model/user_model.dart and lib/model/records_model.dart.

Replace the empty Uri.parse('') with your actual backend URLs.

Generated dart
// Example from lib/model/user_model.dart
final response = await http.Client().post(
    Uri.parse('https://your-api-endpoint.com/login'), // <-- UPDATE THIS
    //...
);
IGNORE_WHEN_COPYING_START
content_copy
download
Use code with caution.
Dart
IGNORE_WHEN_COPYING_END

Run the app

Generated sh
flutter run
IGNORE_WHEN_COPYING_START
content_copy
download
Use code with caution.
Sh
IGNORE_WHEN_COPYING_END

You can also select a target device (e.g., Chrome for web, an emulator for Android) in your IDE and run it from there.

🗄️ Backend Information

The app expects a backend API with the following endpoints:

POST /login: Authenticates a user based on their username.

POST /records/fetch: Fetches records for a given user within a date range.

POST /records/add: Adds a new memorization record.

POST /records/edit: Edits an existing record.

POST /records/delete: Deletes a record by its ID.

You will need to implement a backend server that provides these routes and connects to a database to use the app fully.

📂 Project Structure

The project follows a standard Flutter structure, with the core logic organized as follows:

Generated code
lib/
├── main.dart             # App entry point and main screen (Home)
├── model/
│   ├── records_model.dart  # Data model and API calls for Records
│   └── user_model.dart     # Data model and API calls for Users
└── view/
    └── login_screen.dart   # The UI for the login screen
IGNORE_WHEN_COPYING_START
content_copy
download
Use code with caution.
IGNORE_WHEN_COPYING_END
🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

If you have a suggestion that would make this better, please fork the repo and create a pull request.

Fork the Project

Create your Feature Branch (git checkout -b feature/AmazingFeature)

Commit your Changes (git commit -m 'Add some AmazingFeature')

Push to the Branch (git push origin feature/AmazingFeature)

Open a Pull Request

