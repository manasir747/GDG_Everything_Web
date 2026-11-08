# StudyPortal 🧠✨
### GDG Everything Web — Web Development with React

[![React](https://img.shields.io/badge/React-19.2-61DAFB?logo=react&logoColor=black)](https://react.dev/)
[![Vite](https://img.shields.io/badge/Vite-8.0-646C99?logo=vite&logoColor=white)](https://vitejs.dev/)
[![Google Gemini](https://img.shields.io/badge/Google%20Gemini-2.5%20Flash-4285F4?logo=google&logoColor=white)](https://ai.google.dev/)
[![React Router](https://img.shields.io/badge/React_Router-v7-CA4245?logo=react-router&logoColor=white)](https://reactrouter.com/)

**StudyPortal** is an interactive, modern React application built as part of the **Google Developer Groups (GDG) "Everything Web"** workshop series. It takes learners from foundational React concepts (components, props, state, event handling, and client-side routing) all the way to integrating Generative AI using the **Google Gemini API** (`@google/genai`).

---

## 🚀 Features

### 1. 🤖 AI Quiz Portal (`/quiz`)
- Powered by **Google Gemini 2.5 Flash** via `@google/genai`.
- Enter any topic (e.g., *React Hooks*, *Quantum Computing*, *World History*) to dynamically generate interactive, multiple-choice quizzes.
- Real-time scoring, instant answer feedback, and end-of-quiz score summary.

### 2. 🧪 React Concept Sandbox (`/concepts`)
Interactive mini-apps demonstrating essential React patterns and hooks:
- **🔢 Counter**: State management (`useState`) and increment/decrement event handling.
- **✍️ Live Text Input**: Two-way data binding and controlled form inputs.
- **💡 Light Switch**: Boolean state toggling with dynamic CSS glow effects.
- **🎨 Dynamic Styling (Color Picker)**: State-driven inline styles and color palettes.
- **🚀 Learning List**: Dynamic array state manipulation, list rendering (`.map()`), and unique keys.
- **⚡ Registration Form**: Form submission handling (`onSubmit`), default prevention, and conditional rendering.

### 3. 🌐 Seamless Routing & Navigation
- Multi-page experience powered by **React Router v7** (`react-router-dom`).
- Clean, accessible navigation bar with active route highlighting.

### 4. 🎨 Modern Dark Theme UI
- Styled using the custom [`gdg-ui`](https://github.com/PriyanshusinghPanda/gdgUiLib) design system (`Navbar`, `Button`, `Card`, `Grid`, `Container`, `Input`, `Badge`).
- Sleek glassmorphism aesthetic with responsive layouts.

---

## 🛠️ Tech Stack

- **Frontend**: [React 19](https://react.dev/)
- **Bundler & Dev Server**: [Vite 8](https://vitejs.dev/)
- **Routing**: [React Router DOM v7](https://reactrouter.com/)
- **AI Integration**: [Google Gen AI SDK (`@google/genai`)](https://www.npmjs.com/package/@google/genai) — Gemini 2.5 Flash
- **UI Library**: `gdg-ui`
- **Linting**: ESLint 9

---

## 📂 Project Structure

```text
GDG_Everything_Web/
├── public/                 # Static assets and icons
├── src/
│   ├── assets/             # Project images & logos
│   ├── components/         # Interactive React concept components
│   │   ├── ColorPicker.jsx       # State-driven CSS styling
│   │   ├── Counter.jsx           # Numeric state counter
│   │   ├── LightSwitch.jsx       # Boolean state toggle
│   │   ├── RegistrationForm.jsx  # Form handling & conditional view
│   │   ├── SkillList.jsx         # Array state & list rendering
│   │   └── TextInput.jsx         # Controlled input component
│   ├── lib/
│   │   └── gemini.js       # Google Gemini SDK setup & prompt logic
│   ├── pages/              # Route views
│   │   ├── About.jsx       # About GDG & community pillars
│   │   ├── Concepts.jsx    # Concept sandbox showcase
│   │   ├── Home.jsx        # Landing page & hero section
│   │   └── Quiz.jsx        # AI-powered quiz generator & gameplay
│   ├── App.jsx             # Root layout & route configuration
│   ├── index.css           # Global typography & reset styles
│   └── main.jsx            # Application entry point
├── day3_upgrade_guide.md   # Step-by-step Gemini integration guide
├── index.html              # HTML template
├── package.json            # Dependencies & scripts
└── vite.config.js          # Vite configuration
```

---

## 🏁 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (version 18 or higher recommended)
- [npm](https://www.npmjs.com/) (bundled with Node.js)
- A **Google Gemini API Key** from [Google AI Studio](https://aistudio.google.com/)

---

### Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/manasir747/GDG_Everything_Web.git
   cd GDG_Everything_Web
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure the Gemini API Key**
   Create a `.env` file in the root directory:
   ```bash
   touch .env
   ```
   Add your Gemini API key:
   ```env
   VITE_GEMINI_API_KEY=your_actual_gemini_api_key_here
   ```
   > 💡 *Note: Alternatively, you can set the key directly in `src/lib/gemini.js` for quick local testing.*

4. **Start the development server**
   ```bash
   npm run dev
   ```
   Open your browser and navigate to the local URL shown in your terminal (typically `http://localhost:5173`).

---

## 📜 Available Scripts

| Command | Description |
| :--- | :--- |
| `npm run dev` | Starts the Vite local development server with Hot Module Replacement (HMR). |
| `npm run build` | Compiles and bundles production-ready assets into the `dist/` folder. |
| `npm run preview` | Runs a local web server to preview the production build. |
| `npm run lint` | Runs ESLint to check for code quality and syntax issues. |

---

## 💡 Workshop Progression

This repository represents the culmination of the GDG Web Development bootcamp:

- **Day 1**: Introduction to React components, JSX, props, and layout structure.
- **Day 2**: Mastering React Hooks (`useState`), event handling, controlled inputs, and client-side navigation with `react-router-dom`.
- **Day 3 (The AI Upgrade)**: Integrating Google Gemini (`gemini-2.5-flash`) via the official `@google/genai` SDK to build an intelligent, on-demand quiz generator. Refer to [`day3_upgrade_guide.md`](./day3_upgrade_guide.md) for the live workshop walkthrough.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/manasir747/GDG_Everything_Web/issues).

---

## 📄 License

This project was built for educational purposes as part of Google Developer Groups (GDG) workshops.
