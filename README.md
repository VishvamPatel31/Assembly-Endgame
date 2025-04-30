# 🧠 Assembly: Endgame

A word-guessing game where each incorrect letter eliminates a programming language — lose them all, and you're stuck with Assembly 😱. Built using **React**, this project helped me practice and apply a wide range of core React concepts in a fun and engaging way.

🔗 **Live Demo:** [https://brilliant-longma-12de42.netlify.app](https://brilliant-longma-12de42.netlify.app)

---

## 📚 React Concepts I Practiced

### 🔁 useState
- Used to manage multiple pieces of state:
  - `currentWord`, `guessedLetters`, and game status like win/loss conditions.
- Learned how to update state conditionally and based on previous state.

### 🧠 Derived State Logic
- Computed values like `isGameWon`, `isGameLost`, and `wrongGuessCount` without storing them as state.
- Reinforced how to calculate values from existing state instead of storing everything.

### 🎯 Event Handling
- Attached click events to keyboard buttons with logic to disable them after being used.
- Handled reset via a “New Game” button.

### 🎨 Conditional Rendering
- Rendered win/loss/farewell messages dynamically depending on game state.
- Showed/hid confetti using simple `if` conditions and short-circuiting.

### ✅ Conditional Class Names (with `clsx`)
- Dynamically styled elements like keys and language chips based on correct/incorrect guesses.

### 🔄 Functional State Updates
- Used functional updates inside `setGuessedLetters()` to avoid stale state bugs.

### 🔠 Controlled Rendering with `map()`
- Displayed:
  - Language chips using `map()` over a predefined `languages` array.
  - Keyboard buttons dynamically from the alphabet.
  - Word letters using `.map()` over the selected word.

### ♿ Accessibility with ARIA
- Implemented ARIA roles and visually-hidden screen reader updates for inclusive design.

### 🎉 Component Libraries
- Used `react-confetti` to add celebratory animations on win state.

---

## 🛠️ Tech Stack

- **React**
- **Vite**
- **Netlify** (deployment)
- **CSS / custom styles**
- **clsx** for class management
- **react-confetti** for animations

---

## 📝 How to Run Locally

```bash
git clone https://github.com/your-username/assembly-endgame.git
cd assembly-endgame
npm install
npm run dev
