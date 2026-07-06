# Kotlin Calculator

A simple yet powerful calculator app built with **Jetpack Compose** and **Kotlin**. 
Designed with clean UI, real-time input handling, and robust error management — 
perfect for everyday calculations.

---

## ✨ Features

### Core Operations
- **Basic arithmetic**: Addition (`+`), Subtraction (`-`), Multiplication (`×`), Division (`÷`)
- **Advanced functions**: 
  - Exponentiation (`x^y`) — raise any number to any power
  - Factorial (`n!`) — calculate factorial instantly
  - Square Root (`√x`) — compute square roots
- **Smart input**:
  - Parentheses support for complex expressions: `(2 + 3) × 4`
  - Percentage calculations (`%`) — quick discounts and tips
- **Error handling**:
  - Division by zero → shows clear error message
  - Invalid expressions → prevents crashes
  - Number overflow protection

### User Experience
- **🌙 Dark / ☀️ Light theme** — toggle with one tap
- **Real-time display** — see your expression as you type
- **Responsive layout** — adapts to any screen size
- **Clear and delete** — `C` to clear all, `⌫` to delete last character

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **Kotlin** | Primary programming language |
| **Jetpack Compose** | Modern declarative UI |
| **Material 3** | UI components and theming |
| **ViewModel** | State management with lifecycle awareness |
| **LiveData / StateFlow** | Reactive UI updates |

---

## 📁 Project Structure

The app follows a **simple and maintainable** architecture — clear separation between UI, business logic, and theming:
app/src/main/java/com/example/calculator/
│
├── MainActivity.kt # App entry point, sets up Compose UI
│
├── Calculator.kt # Main screen UI (all Compose components)
│
├── CalculatorViewModel.kt # Business logic & state management
│
└── ui/theme/ # Theme configuration
├── Color.kt # Color palette (light & dark)
├── Theme.kt # Material 3 theme setup
└── Type.kt # Typography styles

text

### Why this structure?

- **`MainActivity`** → Hosts the Compose UI, sets the theme
- **`Calculator.kt`** → Contains all UI components (buttons, display, layouts)
- **`CalculatorViewModel.kt`** → Handles all calculations, input validation, and state
- **`ui/theme/`** → Centralized theming for easy dark/light mode switching

This approach keeps the code:
- ✅ **Organized** — each file has a single responsibility
- ✅ **Testable** — ViewModel logic can be unit-tested
- ✅ **Scalable** — easy to add new features without chaos

---

## 🎯 How to Use

| Action | What it does |
|--------|--------------|
| `0-9` | Enter digits |
| `+ - × ÷` | Select operation |
| `=` | Calculate the result |
| `C` | Clear everything |
| `⌫` | Delete last character |
| `( )` | Add parentheses |
| `%` | Percentage calculation |
| `x^y` | Raise to power |
| `n!` | Factorial |
| `√` | Square root |
| `🌙/☀️` | Toggle dark/light theme |

---

## 🚀 Getting Started

### Prerequisites
- Android Studio Iguana (2023.2.1) or newer
- JDK 17+
- Android SDK 24+ (Android 7.0+)

### Run the app

1. **Clone** the repository:
   ```bash
   git clone https://github.com/EeXoMe/Calculator.git
Open the project in Android Studio

Sync Gradle files

Run on emulator or physical device (API 24+)

📱 Screenshots
Add your screenshots here:

Light Theme	Dark Theme
(add light_theme.png)	(add dark_theme.png)
🧪 Error Handling
The calculator gracefully handles edge cases:

Scenario	What happens
5 ÷ 0	Shows Error: Cannot divide by zero
2 + (3 × (missing bracket)	Auto-fixes or shows error
9999999999 × 9999999999 (overflow)	Shows Error: Number too large
Empty expression + =	Does nothing (no crash)
🔮 Future Improvements
Planned features to make the app even better:

Calculation history — store and recall last 20 results

Keyboard support — use physical keyboard for faster input

Copy to clipboard — one-tap copy results

Unit tests — test all calculator logic with JUnit

UI tests — test button clicks with Compose UI Testing

Voice input — speak calculations using Speech-to-Text (Android API)

Export history — save calculations as text file

Scientific mode — trigonometric functions (sin, cos, tan)

🤝 Contributing
This is a learning project, but feedback is always welcome!
Feel free to:

Open an issue with suggestions

Fork the repo and experiment

Reach out if you're hiring! 😊

👨‍💻 Author
Artyom Gilmutdinov

GitHub: @EeXoMe

Open to Android Developer (Junior) roles

Passionate about Kotlin, Compose, and clean code
