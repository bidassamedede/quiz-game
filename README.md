# Quiz Game

## Project Description
The **Quiz Game** is an interactive web-based game where players can test their knowledge on various topics. The game presents a series of questions, and users can select one of the multiple-choice options. The game provides feedback on the selected answer and shows the user's score at the end. It also includes a feature to restart the quiz.

## Project Structure

The project consists of three primary files:

1. **index.html** - The main HTML file that contains the structure of the game.
2. **style.css** - The CSS file that defines the styling of the game interface.
3. **questions.json** - A JSON file containing the quiz questions, options, and correct answers.

### File Breakdown

#### index.html
This file contains the structure of the quiz game, which includes:
- A header (`<h1>`) for the title of the game.
- A dynamic section that presents questions, options, and feedback to the user using Vue.js.
- A section to display the final score after completing the quiz.

**Features**:
- Uses Vue.js for dynamic updates and interactions.
- Displays one question at a time.
- Provides feedback after each answer and shows the final score at the end.
- Allows the user to restart the quiz once finished.

#### style.css
This CSS file handles the layout and design of the quiz game, ensuring it is visually appealing and user-friendly. 

**Key Styles**:
- Centers the game interface on the screen.
- Provides interactive styles for list items and buttons (hover effects).
- Defines colors and spacing for readability.

#### questions.json
A JSON file that contains an array of quiz questions. Each question is an object with:
- `id`: A unique identifier for the question.
- `question`: The text of the question.
- `options`: An array of answer choices.
- `answer`: The correct answer for the question.

Example:
```json
[
  {
    "id": 1,
    "question": "Which keyword is used to declare a variable in JavaScript?",
    "options": ["var", "let", "const", "All of the above"],
    "answer": "All of the above"
  }
]
```

## How to Run the Project

1. **Clone the repository**:
   - Clone this project to your local machine.
   ```bash
   git clone <repo_url>
   ```

2. **Run the Project**:
   - Open the `index.html` file in any modern web browser (e.g., Chrome, Firefox).

3. **Gameplay**:
   - Click on an answer option to check if it's correct.
   - After each answer, feedback will appear.
   - Once all questions have been answered, the score is shown.
   - You can restart the quiz by clicking the "Restart" button.

## Technologies Used
- **HTML**: Used for the structure of the web page.
- **CSS**: Used for styling the quiz game.
- **Vue.js**: Used for handling dynamic content and interactivity.
- **JSON**: Used to store the quiz questions, options, and answers.

## How the Game Works

1. **Loading Questions**:
   - The questions are loaded asynchronously from the `questions.json` file using the `loadQuestions()` method.
   
2. **Answering Questions**:
   - The user selects an answer by clicking on one of the listed options.
   - The `checkAnswer()` method compares the selected answer to the correct answer and provides feedback.

3. **Feedback and Score**:
   - After the user selects an answer, the game shows whether it was correct or wrong.
   - The score is updated for each correct answer.
   
4. **End of Game**:
   - When all questions have been answered, the quiz displays the total score.
   - The user can restart the quiz by clicking the "Restart" button.

## Example of a Question in JSON Format

```json
{
  "id": 1,
  "question": "Which keyword is used to declare a variable in JavaScript?",
  "options": ["var", "let", "const", "All of the above"],
  "answer": "All of the above"
}
```

## How to Customize the Quiz

- **Adding New Questions**: 
  - You can modify the `questions.json` file to add more questions. Just follow the format of the existing questions.
  
- **Changing the Look and Feel**:
  - Modify the `style.css` to customize the quiz's appearance, including colors, fonts, and layout.

- **Adding More Features**:
  - You can extend the game by adding timers, difficulty levels, or saving high scores.

## License
This project is open-source and free to use under the MIT License.

## Troubleshooting
If you encounter issues with loading questions, ensure that the `questions.json` file is in the correct path and properly formatted. If the game is not functioning as expected, check the browser console for any errors.

