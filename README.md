# InkFlow - Book Reading & Writing Platform

InkFlow is a comprehensive Flutter-based mobile application that provides a fully-featured platform for reading and writing books. Readers can browse through a large collection of books, follow their favorite authors, maintain a personal library, and track their reading analytics. Writers are provided with a dedicated suite of tools to create and publish stories, manage chapters, and even use AI to suggest creative book titles. The app is seamlessly integrated with Firebase for its robust backend, including authentication, real-time database, analytics, and AI capabilities.

## Features

### For Readers
- **Book Discovery**: Browse through a collection of books with detailed views and cover images.
- **Author Following**: Explore author profiles and follow favorite authors to stay updated with their new releases.
- **Personal Library**: Save books to your personal library for easy access.
- **Reading Analytics**: Track progress and engagement with detailed reading analytics.
- **Search Functionality**: Discover new books and authors with the integrated search bar.
- **Content Purchasing (UI Demo)**: Simulated purchase flow for premium chapters featuring mocked payment validation (Bank, JazzCash, EasyPaisa). No real transactions occur.

### For Writers
- **Book Creation**: Create new books with a title, description, and cover image.
- **AI Title Generation**: Utilize Gemini AI (via `firebase_ai`) to auto-generate creative and catchy book titles based on story descriptions.
- **Chapter Management**: Add, modify, and publish structured chapters for your books.
- **Content Pricing & Analytics**: Set prices for premium chapters and monitor reading analytics for tracking engagement.
- **Writing Dashboard**: A unified dashboard to manage all your written content.

### Backend & Security
- **Firebase Authentication**: Secure account creation and login flow.
- **Realtime Database**: Live syncing for user data, books, and purchases.
- **Firebase Crashlytics & Analytics**: Monitoring performance, usage statistics, and application stability.

---

## Screenshots

<table align="center">
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/0c25af0b-6087-4ad2-8e4a-5922fbed0e8c" width="200"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/e0749496-3b67-4106-8797-70d6a8f6f463" width="200"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/02cda46d-21e5-403b-ab87-b9aee11c2fbd" width="200"/>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/6c2f8251-f651-4002-9c94-cb7d3065be55" width="200"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/7990a5e9-a0e6-41a3-8d8d-58b4e4dff310" width="200"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/0c11f4ef-b460-4684-baf8-45a0a61c7f49" width="200"/>
    </td>
  </tr>
  <tr>
    <td align="center" colspan="3">
      <img src="https://github.com/user-attachments/assets/9114a943-3e51-47a0-b0ea-98cdb41ee77b" width="200"/>
    </td>
  </tr>
</table>

---

## Technologies Used
- **Framework**: Flutter
- **Language**: Dart
- **Backend/BaaS**: Firebase (Auth, Realtime Database, Analytics, Crashlytics)
- **AI**: Firebase AI (Gemini Flash Model)
- **UI Components**: Material Design
- **Packages**:
  - `firebase_core`, `firebase_auth`, `firebase_database`, `firebase_analytics`, `firebase_crashlytics`
  - `firebase_ai` — For Gemini AI generative text prompts
  - `google_fonts` — For customized typography
  - `standard_searchbar` — For search functionality
  - `image_picker`, `image` — For selecting and managing book cover images and avatars

---

## Installation and Setup

### Prerequisites
- Flutter SDK (^3.7.0)
- Android Studio or VS Code
- A configured Firebase project (`google-services.json` and `GoogleService-Info.plist` correctly placed)

### Steps

1. Clone the repository
   ```bash
   git clone https://github.com/Romaisa-Munir/inkflow_mad_sem_project.git
   ```

2. Navigate to the project directory
   ```bash
   cd inkflow_mad_sem_project
   ```

3. Install dependencies
   ```bash
   flutter pub get
   ```

4. Run the app
   ```bash
   flutter run
   ```

---

## Project Structure

```
lib/
├── data/                    # Sample data
├── models/                  # Data models (Author, Book, Chapter)
├── pages/
│   ├── Analytics/           # Book reading analytics views
│   ├── authors/             # Author profiles and discovery pages
│   ├── books/               # Book listing, detailing, and reading interface
│   ├── home/                # Main home screen
│   ├── library/             # User's personal library
│   ├── login_signup/        # Authentication screens
│   ├── payment/             # Payment processing dialogs
│   ├── profile/             # User profile and settings
│   ├── AddChapterPage.dart  # Form for writers to add chapters
│   ├── BookDetailsPage.dart # Main display of a book
│   ├── create_book_page.dart# Form to initiate a new book
│   └── writing_dashboard.dart # Central hub for writers
├── services/                # Backend interaction (AI, Author, Payment, Reading Analytics)
├── theme/                   # Global app theme and styling
├── widgets/                 # Reusable UI components (book_card, chapter_card)
├── firebase_options.dart    # Firebase config setup
└── main.dart                # Application entry point & routing
```

---

## Contributors

- **Romaisa Munir** — [@Romaisa-Munir](https://github.com/Romaisa-Munir)
- **Warda Khan** — [@wardakhan0101](https://github.com/wardakhan0101)

---

## License

This project is for educational purposes.
