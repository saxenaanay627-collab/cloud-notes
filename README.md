# cloud-notes
 Cloud Notes (Real-time Sync)
A lightweight, web-based notebook application that stores data in the cloud using Firebase Firestore. This app allows users to create and delete notes with instant synchronization across all devices without needing a page refresh.

Features:
Real-time Synchronization: Uses Firebase onSnapshot to listen for database changes and update the UI instantly.
Cloud Storage: Data is stored securely in Google Cloud (Firestore), not locally on the browser.
Persistent Data: Notes remain available even if you clear your browser cache or switch computers.
Zero-Installation: Runs directly in any modern web browser using the Firebase CDN.

Built With
HTML5 & CSS3: For the structure and responsive styling.
JavaScript (ES6 Modules): For the application logic.
Firebase Firestore: NoSQL cloud database for real-time data management.

How It Works
1. The Database Structure
The app creates a collection in Firestore called notes. Each document in this collection contains:
text: The content of your note.
timestamp: The server-side time when the note was created (used for sorting).
