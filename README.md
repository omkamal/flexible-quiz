# Flexible Quiz

Flexible Quiz is a Vue.js application designed to generate interactive HTML quizzes from JSON files. This application allows users to upload a JSON file containing quiz questions and answers, which are then rendered into a user-friendly quiz interface.

## Features

- **Dynamic Quiz Generation**: Load quizzes dynamically from JSON files.
- **Interactive UI**: Provides an engaging user interface with real-time feedback on answers.
- **Performance Tracking**: Displays scores and time spent on each question.
- **Review Incorrect Answers**: Offers explanations for incorrect answers to enhance learning.

## Getting Started

### Prerequisites

- Ensure you have a modern web browser installed.
- No additional software is required to run the application.

### Usage

1. **Upload a Quiz**: Click on "Choose Quiz File" to upload a JSON file containing your quiz.
2. **Start the Quiz**: Once the quiz is loaded, click "Start Quiz" to begin.
3. **Answer Questions**: Select your answer for each question and receive immediate feedback.
4. **View Results**: After completing the quiz, view your score and review any incorrect answers.

### JSON File Format

The JSON file should follow this structure:

```json
{
    "title": "Quiz Title",
    "questions": [
        {
            "id": 1,
            "text": "Question text",
            "choices": ["Choice 1", "Choice 2", "Choice 3", "Choice 4"],
            "answers": {
                "correct": {"index": 0, "comment": "Explanation for correct answer"},
                "wrong": [
                    {"index": 1, "comment": "Explanation for wrong answer"},
                    {"index": 2, "comment": "Explanation for wrong answer"},
                    {"index": 3, "comment": "Explanation for wrong answer"}
                ]
            }
        }
    ]
}
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Built with [Vue.js](https://vuejs.org/)
- Math rendering powered by [MathJax](https://www.mathjax.org/)
- Charting provided by [Chart.js](https://www.chartjs.org/)
