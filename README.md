# Quiz Vue

> A Vue.js project for creating and managing quizzes.

## Project Description

Quiz Vue is a simple quiz application built using Vue.js. It allows users to navigate through a series of questions, select answers, and review their choices. The project is designed to be lightweight and easy to set up, making it ideal for educational purposes or quick prototyping.

### Key Features
- **Dynamic Question Navigation**: Users can move forward and backward through questions.
- **Answer Selection**: Users can select answers and review their choices.
- **Responsive Design**: Built with Bootstrap for a responsive and modern UI.
- **Vue.js Components**: Modular components for easy maintenance and scalability.

---

## Project Structure

The project is organized as follows:

```
quiz-vue/
├── .babelrc                # Babel configuration for JavaScript transpilation
├── .editorconfig           # Editor configuration for consistent coding styles
├── .gitignore              # Specifies files and directories to ignore in Git
├── index.html              # Main HTML file for the application
├── package.json            # Project dependencies and scripts
├── README.md               # Project documentation (this file)
├── App.vue                 # Root Vue component
├── Header.vue              # Header component
├── Test.vue                # Test component for displaying questions
├── questions.json          # JSON file containing quiz questions and answers
├── main.js                 # Entry point for the Vue application
├── vue.config.js           # Vue-specific configuration
├── webpack.config.js       # Webpack configuration for bundling
```

---

## Tech Stack & Dependencies

### Core Technologies
- **Vue.js**: A progressive JavaScript framework for building user interfaces.
- **Bootstrap**: A CSS framework for responsive and modern UI components.
- **Webpack**: A module bundler for JavaScript and other assets.
- **Babel**: A JavaScript compiler for using modern JavaScript features.

### Dependencies
- **vue**: `^2.5.11`
- **bootstrap**: `^5.2.3`
- **vue-loader**: `^13.0.5`
- **vue-template-compiler**: `^2.4.4`
- **webpack**: `^3.6.0`
- **webpack-dev-server**: `^2.9.1`

### Development Dependencies
- **babel-core**: `^6.26.0`
- **babel-loader**: `^7.1.2`
- **babel-preset-env**: `^1.6.0`
- **babel-preset-stage-3**: `^6.24.1`
- **cross-env**: `^5.0.5`
- **css-loader**: `^0.28.7`
- **file-loader**: `^1.1.4`

---

## Installation & Setup

### Prerequisites
- Node.js (v14 or higher recommended)
- npm (Node Package Manager)

### Steps
1. **Clone the repository**:
   ```bash
   git clone https://github.com/hasankoman/quiz-vue.git
   cd quiz-vue
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Run the development server**:
   ```bash
   npm run dev
   ```
   The application will be available at `http://localhost:8080`.

4. **Build for production**:
   ```bash
   npm run build
   ```
   The production-ready files will be generated in the `dist/` directory.

---

## Usage Guide

### Running the Application
- Use `npm run dev` to start the development server with hot reload.
- Use `npm run build` to generate a production build.

### Navigating the Quiz
- Use the "Devam Et" (Continue) button to move to the next question.
- Use the "Önceki" (Previous) button to go back to the previous question.
- Select an answer by clicking on the corresponding button.

---

## Contribution Guidelines

Contributions are welcome! If you'd like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes with clear and descriptive messages.
4. Submit a pull request.

### Coding Style
- Follow the existing code style (2-space indentation, ES6 syntax).
- Ensure all new code is properly documented.

---

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## Author

- **Hasan Koman**  
  Email: [hasankoman94@gmail.com](mailto:hasankoman94@gmail.com)  
  GitHub: [hasankoman](https://github.com/hasankoman)

---

For more details on Vue.js, check out the [official Vue.js documentation](https://vuejs.org/v2/guide/).