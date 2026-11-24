# 📖 Digital Reading App for University Students

ReadOn is a cross-platform mobile reading app that helps university students read academic books, articles, and journals **more deeply**, not just faster. On top of a standard reading experience, it adds tools for self-regulated learning: daily reading goals, comprehension tracking, quizzes, collaborative notes, and reviews.

> **Portfolio project.** This repository is a showcase only. The source code is private and is not open source.

## 🎬 Demo
https://youtube.com/shorts/hknS_F5frd0?feature=share

<!-- Optional: add a clickable thumbnail
[![ReadOn Demo](docs/thumbnail.png)](YOUR_DEMO_VIDEO_LINK_HERE)
-->

## 🎯 Why ReadOn?

Many students skim academic texts, struggle to find time for required readings, and rarely reflect on what they have read. Short-form content habits make it harder to keep focus on long texts. ReadOn addresses this by combining a digital library with features that encourage planning, monitoring, and reflection while reading.

## ✨ Features

### 👤 Account & Profile
- **Register and login** with email and password, with input validation and clear error messages.
- **Profile page** showing name, email, and the total number of books, articles, and journals read.
- **Edit profile**: update profile picture, username (must be unique), and full name through a popup form.

### 🔎 Discover & Search
- **Discover** reading material by **type** (book, article, journal) and **genre**.
- **Search** by keyword, with **Top Searches** and **Recent Searches**. Recent keywords can be tapped to search again or deleted.
- Open an **item detail page** from any result, with a "no results found" state when nothing matches.
- Tap the **heart icon** to add an item to your favorites.
- **Upload your own reading files** (PDF or Word) with form validation (empty fields, unsupported file format, invalid page count).

### 📚 My Library
- View your reading list organized by **status** (currently reading, finished) and **favorites**.
- Jump straight into the reader from your library.

### 📖 Reading Experience
- **Continue where you left off**: the reader opens at your last read page, or page 1 for new items.
- **Next / previous page** navigation.
- **Highlight text** and review all highlights in a bottom sheet, with the option to delete them one by one or all at once.
- **Bookmarks**: tap the bookmark icon to save or remove a page, and open the **Bookmarks page** to see all your saved pages as cards that take you straight back to the page.

### 🎯 Reading Goals & Progress
- **Set a daily reading goal** per item, either as *pages per day* or as a *target finish date*. For the date option, the app calculates the daily pages from the remaining pages and days.
- Goal values are validated (not less than 1, not above the remaining pages, no past dates).
- **Live progress bar** inside the reader showing today's start page, today's target page, and the achievement percentage.
- Reading sessions (start page, end page, reading time) are saved automatically when you close the reader, and the day's result is updated.

### 🧠 Comprehension Tools
- **Mark Confused**: select text you do not understand and flag it. The page and text position are saved and the text is visually marked.
- **Create Checkpoint**: after finishing a section, explain it in your own words and rate your confidence (*Not Understood Yet*, *Fair*, *Understand*).
- **Comprehension Notes**: review all confused sections and low-confidence checkpoints sorted by page, jump back to the exact page, and update your understanding.

### 📝 Quizzes
- Browse available quizzes and answer questions about a reading.
- An **optional quiz pop-up** can appear when opening a reading from My Library.
- Leaving a quiz midway **saves your progress** and moves it to the *Ongoing* category.
- Confirm before submitting, then see your score instantly.

### 🗒️ Notes & Collaboration
- Create notes linked to a book, article, or journal, including the page number and file attachments.
- **Pin** important notes, edit note details and content.
- **Collaboration Notes**: invite other users to collaborate and view notes that others shared with you.

### ⭐ Reviews & Ratings
- Rate finished items from **1 to 5 stars** with a written review (the review button only appears after you finish reading).
- Browse reviews from other readers by item, search or filter by category (articles, journals, books), and filter reviews by star rating.

### 🏆 Leaderboard
- See the **top three readers**, your own rank, and the ranking of other users, based on the total number of items read.

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Mobile app (frontend) | Flutter, Dart |
| Backend | Node.js, Express.js, JavaScript |
| Database | MySQL |
| Architecture | MVC (Model–View–Controller) |

## 🏗️ Architecture

The app follows the **MVC** pattern. Each feature (authentication, discover, library, bookmarks, reading goals, comprehension notes, notes, reviews, quizzes, leaderboard) has its own **View** (UI), **Controller** (handles user actions and business flow), and **Model** (data and validation rules), which keeps the codebase organized and easy to extend.

## 🎓 Project Context

ReadOn was developed as part of my final-year Computer Science undergraduate thesis at **BINUS University, Jakarta**, focusing on supporting deep reading and self-regulated learning for undergraduate students.

## 📄 License

© All rights reserved. This project is shared for portfolio purposes only. The source code is private, and copying, redistribution, or reuse is not permitted without permission.
