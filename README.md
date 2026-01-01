📘 Vocabulary Learning App

A modern vocabulary learning web application that allows users to explore words by level, view detailed meanings, hear pronunciations, search vocabularies, and save favorite words — all powered by APIs and an interactive UI inspired by Figma designs.

🚀 Features
🔢 Level-Based Learning

Center-aligned heading as per Figma design

Dynamically generated Lesson/Level buttons from API-01

Lesson buttons load automatically on page load

Active lesson button is visually highlighted

📚 Vocabulary Cards

Default instructional text shown initially

Clicking a lesson loads words from API-02

Each word card displays:

Word

Meaning & pronunciation

Action buttons with icons (as per Figma)

Displays “No Word Found” if a lesson has no data

🎨 Active Level Indicator

Active lesson button changes color after successful data load

Helps users easily identify the current level

🪟 Vocabulary Details Modal

Modal opens when clicking the details icon

Loads detailed data from API-03

Modal displays:

Word with pronunciation

Example sentence

Synonyms

“Complete Learning” button to close modal

⚠️ Invalid Data Handling

Prevents displaying null, undefined, or empty values

Shows fallback or relevant text if data is missing

⏳ Loading Spinner

Loading spinner appears while vocabulary data is being fetched

Improves user experience during API calls

🔍 Search Functionality

Search input to filter vocabulary words

Real-time search results shown on input change

Searching automatically resets the active lesson button

❤️ Save Word Feature

Heart icon added to vocabulary cards

Users can save favorite words

Saved words are displayed in a separate Saved Section

🔊 Speak Your Vocabulary

Pronunciation feature using Web Speech API

Click sound icon to hear word pronunciation

function pronounceWord(word) {
  const utterance = new SpeechSynthesisUtterance(word);
  utterance.lang = "en-EN";
  window.speechSynthesis.speak(utterance);
}

🛠️ Technologies Used

HTML

CSS

JavaScript

REST APIs

Web Speech API

📡 APIs Used

API-01 → Fetch lesson/level list

API-02 → Fetch vocabulary words by lesson

API-03 → Fetch detailed vocabulary information

📦 Installation & Setup
git clone 
cd vocabulary-


Open index.html in your browser or use a live server.

🎯 Future Improvements

User authentication

Persistent saved words using localStorage / database

Pagination for large vocab lists

Mobile optimization

🙌 Acknowledgements

UI inspired by Figma design

Built for learning, practice, and vocabulary improvement

👤 Author

Motahar Hossain Mohim
