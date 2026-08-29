# Persistent Sticky Notes Corkboard

## Description
A digital Sticky Notes dashboard that allows users to create reminders and pin them to a virtual corkboard. Unlike standard temporary web apps, this project utilizes the browser's **Web Storage API (LocalStorage)** to persist data. Any notes created are saved locally, meaning they will survive tab closures, page refreshes, and browser restarts.

## Features
- Add text-based sticky notes to a responsive grid.
- Unique IDs generated for each note using `Date.now()`.
- Data persistence using `localStorage`, `JSON.stringify()`, and `JSON.parse()`.

## How to Run
1. Clone this repository or download the files to your local machine.
2. Open the `sticky-notes.html` file directly in any modern web browser (Chrome, Firefox, Edge, Safari).
3. No build tools, servers, or external dependencies are required.

## AI Tools & Prompts Used
**AI Tool:** [Insert ChatGPT/Claude/Gemini here]

**Prompt Used to generate utility functions:**
> "Act as an introductory JavaScript instructor. I am building a project where I track an array of objects called notesState. Each object represents a note element looking like this: { id: 1717300000000, content: "Hello world" }.
> Write two JavaScript functions:
> saveNotesToStorage(notesArray): This function accepts the notes array, uses JSON.stringify() to turn the array into a clean JSON text string, and saves it inside the browser's LocalStorage under the key name "boardNotesData".
> loadNotesFromStorage(): This function reads from LocalStorage under the key name "boardNotesData". If data exists, it must use JSON.parse() to transform that JSON string back into a real, live JavaScript array and return it. If the storage key is completely empty or doesn't exist yet, it should return an empty array [].
> Keep the configurations beginner-friendly, utilize descriptive code, and provide only the JavaScript code blocks. Do not add event handlers or DOM manipulations yet."
