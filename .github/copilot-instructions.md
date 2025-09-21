# Copilot Instructions for AI Coding Agents

## Project Overview
This is a simple web-based quiz application. The codebase consists of HTML, CSS, and JavaScript files, with each major page as a separate HTML file. There is no build system, backend, or package management—everything runs client-side in the browser.

## Key Files & Structure
- `Quizzes.html`: Main quiz interface. Loads questions and interacts with `Quizzes.js`.
- `Quizzes.js`: Core quiz logic—question handling, scoring, navigation, and DOM manipulation.
- `Quizzes.css`: Styles for all quiz-related pages.
- `results.html`: Displays quiz results.
- `start quiz.html`: Entry point for starting a quiz.
- `home.html`, `contact.html`, `instructions.html`: Supporting pages for navigation and information.

## Patterns & Conventions
- **Page Navigation**: Each HTML file is a standalone page. Navigation is handled via `<a>` tags or JavaScript redirects.
- **State Management**: Quiz state (current question, score, etc.) is managed in-memory in `Quizzes.js`. No persistent storage is used.
- **DOM Access**: All dynamic UI updates are performed via direct DOM manipulation in `Quizzes.js`.
- **Styling**: All styles are centralized in `Quizzes.css`. Inline styles are discouraged.
- **File Naming**: HTML files use lowercase or spaces; JS/CSS files use PascalCase.

## Developer Workflows
- **Testing**: Manual—open HTML files in a browser and interact with the UI. No automated tests or test runner.
- **Debugging**: Use browser DevTools (console, inspector) to debug JavaScript and inspect DOM.
- **Adding Questions**: Update question data structures in `Quizzes.js`.
- **Customizing Styles**: Edit `Quizzes.css` for global changes.

## Integration Points
- No external libraries or frameworks are used.
- No backend or API calls—everything is static and client-side.

## Examples
- To add a new quiz, create a new HTML file and update `Quizzes.js` to handle its logic.
- To change scoring, modify the relevant functions in `Quizzes.js`.

## Recommendations for AI Agents
- Always check `Quizzes.js` for core logic changes.
- Keep UI consistent by updating `Quizzes.css` for style changes.
- When adding new features, follow the pattern of standalone HTML pages and update navigation links accordingly.
- Avoid introducing build tools or external dependencies unless explicitly requested.

---
_Last updated: September 19, 2025_
