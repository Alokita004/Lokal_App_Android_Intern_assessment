# Lokal Jobs App 📱

A Jetpack Compose-based Android application built as part of the Lokal App Android Intern Assessment.  
This app showcases job listings fetched from a remote API, supports bookmarking with offline storage using Room, and maintains clean architecture and UI states.





 ✅ Features

- 📄 **Job Listings**: Fetches job listings from the provided Lokal API using infinite scroll.
- 🔍 **Detailed View**: Tap on any job to view more details including salary, location, phone, and description.
- 📌 **Bookmarking**: Bookmark your favorite jobs.
- 📶 **Offline Support**: Bookmarked jobs are saved using Room database for offline access.
- 🔁 **State Management**: Displays appropriate UI states for loading, error, and empty data.
- 🔽 **Bottom Navigation**: Easily switch between “Jobs” and “Bookmarks” screens.

Tech Stack

- **Language**: Kotlin
- **UI**: Jetpack Compose
- **Navigation**: Navigation Compose
- **Networking**: Retrofit + Gson
- **Persistence**: Room Database
- **Architecture**: MVVM
- **Coroutines**: Kotlin Coroutines for async operations




## 🔗 API Reference

- Base URL: `https://testapi.getlokalapp.com/`
- Endpoint: `/common/jobs?page=1`



## 📁 Project Structure

```plaintext
├── model/
│   ├── Job.kt
│   └── BookmarkedJob.kt
├── network/
│   └── JobApiService.kt
├── database/
│   ├── JobDao.kt
│   └── BookmarkedJob.kt
├── repository/
│   └── JobRepository.kt
├── viewmodel/
│   └── JobViewModel.kt
├── ui/
│   ├── JobListScreen.kt
│   ├── JobDetailScreen.kt
│   ├── BookmarkScreen.kt
│   └── JobCard.kt
├── navigation/
│   └── Navigation.kt
└── MainActivity.kt
