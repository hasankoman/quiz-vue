# Quiz Vue

> A Vue.js-based quiz application

## Project Description

**Quiz Vue** is a simple quiz application built using Vue.js. It allows users to answer a series of questions and navigate through them using "Previous" and "Next" buttons. The application is designed to be lightweight, responsive, and easy to use.

### Key Features:
- Dynamic question navigation.
- Responsive design using Bootstrap.
- State management for tracking user answers.
- Easy-to-extend question database.

---

## Project Structure

The project is organized as follows:

```
quiz-vue/
├── .babelrc                # Babel configuration file
├── .editorconfig           # Editor configuration for consistent coding styles
├── .gitignore              # Specifies files and folders to be ignored by Git
├── README.md               # Project documentation
├── dist/                   # Compiled and bundled files for production
│   ├── build.js            # Main JavaScript bundle
│   └── build.js.map        # Source map for debugging
├── index.html              # Main HTML file
├── package.json            # Project dependencies and scripts
├── package-lock.json       # Lock file for dependency versions
├── src/                    # Source code directory
│   ├── App.vue             # Main Vue component
│   ├── assets/             # Static assets (e.g., images)
│   │   └── logo.png        # Application logo
│   ├── components/         # Vue components
│   │   ├── Header.vue      # Header component
│   │   └── Test.vue        # Quiz component
│   ├── database/           # Data files
│   │   └── questions.json  # JSON file containing quiz questions
│   └── main.js             # Entry point for the Vue application
├── vue.config.js           # Vue CLI configuration
└── webpack.config.js       # Webpack configuration for bundling
```

---

## Tech Stack & Dependencies

### Core Technologies:
- **Vue.js** (v2.5.11) - Progressive JavaScript framework.
- **Bootstrap** (v5.2.3) - CSS framework for responsive design.
- **Webpack** (v3.6.0) - Module bundler.

### Development Dependencies:
- **Babel** - Transpiler for modern JavaScript.
- **Vue Loader** - Webpack loader for Vue components.
- **Cross-Env** - Environment variable management.
- **CSS Loader** - Webpack loader for CSS files.
- **File Loader** - Webpack loader for static assets.

---

## Installation & Setup

### Prerequisites:
- Node.js (v14 or higher)
- npm (v6 or higher)

### Steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/hasankoman/quiz-vue.git
   cd quiz-vue
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```
   The application will be available at `http://localhost:8080`.

4. Build for production:
   ```bash
   npm run build
   ```
   The production-ready files will be generated in the `dist/` folder.

---

## Usage Guide

### Running the Application:
- Use `npm run dev` to start the development server with hot reload.
- Use `npm run build` to generate optimized production files.

### Navigating the Quiz:
- Click on an answer to select it.
- Use the "Previous" and "Next" buttons to navigate between questions.
- Click "Tamamla" (Finish) on the last question to complete the quiz.

---

## Contribution Guidelines

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bugfix:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request.

### Coding Style:
- Follow the existing code style (2-space indentation, ES6 syntax).
- Ensure all changes are linted and tested.

---

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## Author

- **Hasan Koman**  
  Email: [hasankoman94@gmail.com](mailto:hasankoman94@gmail.com)  
  GitHub: [hasankoman](https://github.com/hasankoman)

---

For more details on Vue.js, check out the [official documentation](https://vuejs.org/v2/guide/).