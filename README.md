clarityX 🌌

clarityX is an impossibly smooth, AI-powered text refinement application built with React and Tailwind CSS. It is designed to take your messy, unstructured thoughts and instantly transform them into clear, natural, and human-sounding text.

Built with a gorgeous, dark-mode glassmorphism UI, clarityX gets out of your way and focuses entirely on the "Paste → Fix → Done" workflow, while hiding immense power inside its sidebar.

🚀 Features

Core Experience

The "Human" Algorithm: Built on top of the Gemini API, clarityX uses hard-coded "Gold Standard" prompt engineering. It doesn't just fix grammar—it tightens phrasing, removes redundancies, and ensures the output sounds conversational and real, never robotic.

Immersive Glassmorphism UI: Features a dynamic, slowly animating cosmic background with deep blurred panels (backdrop-filter) and custom pulsing neon typography.

Instant Auto-Fix: Toggle "Auto-Fix" on, and the app will quietly polish your text in the background as you type (using intelligent debouncing).

Advanced Tooling (The Hamburger Menu)

Tone Control: Choose from Natural, Casual, Professional, Friendly, Confident, or Persuasive.

Rewrite Strength: Dictate the AI's boundaries (Light fixes, Medium balance, or Strong rewrites).

Length & Language: Force Short, Balanced, or Detailed outputs, in American or British English.

Custom Instructions & Protected Words: Tell the AI exactly what you want (e.g., "Make it sound like a text message") and protect specific brand names or slang from being altered.

Local History: The app saves your last 10 input/output generations locally so you never lose a great rewrite.

Quality of Life Additions

One-Click Simplify 🪄: A magic wand button on the output pane instantly forces a "Short, Casual, Strong" rewrite to make complex text instantly readable.

Dynamic Readability Score: Instantly tells you if your text is Easy, Medium, or Advanced to read.

Export Options: 1-click Copy, Download to .txt, or native Web Share API integration.

Word Count Guardian: Automatically tracks your inputs and enforces a 5,000-word limit to ensure lightning-fast processing.

🛠️ Tech Stack

Frontend Framework: React (using Hooks: useState, useEffect, useRef)

Styling: Tailwind CSS (with custom inline keyframes for blob animations and glassmorphism)

Icons: Lucide React

AI Engine: Google Gemini API (gemini-2.5-flash)

💻 How to Run Locally

Clone the repository:

git clone [https://github.com/yourusername/clarityX.git](https://github.com/yourusername/clarityX.git)
cd clarityX


Install dependencies:
Ensure you have a React environment set up (like Vite or Create React App) with Tailwind CSS installed.

npm install
npm install lucide-react


Add your API Key:
Open App.jsx and locate the handleImproveText function. Find the apiKey variable and insert your Google Gemini API key:

const apiKey = "YOUR_GEMINI_API_KEY_HERE";


(Note: In a production environment, you should move this to a .env file and fetch it securely).

Start the development server:

npm run dev
# or
npm start


🧠 How the "Natural" Tone Works Under the Hood

clarityX is specifically engineered to avoid the "AI-generated" tone that plagues most writing tools. When set to the default "Natural" tone, the system injects a Gold Standard Example into the AI's system instructions:

"I had a hard time explaining what happened yesterday, and I probably made things more confusing than they needed to be. For example, when I talked about the meeting, I was really trying to focus on how people reacted, but I didn’t make that clear, so it just sounded like I was complaining..."

By forcing the AI to use this specific paragraph as its benchmark for pacing, vocabulary, and transition-smoothing, clarityX ensures that your output always sounds like a real human wrote it.

📝 License

Distributed under the MIT License. Feel free to use, modify, and build upon this project!
