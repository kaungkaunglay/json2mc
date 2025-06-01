# 📚 アニメ教育クイズ Book Edition ✨

Welcome to the Anime Education Quiz! This is a simple, interactive web-based quiz system that uses JSON input to generate multiple-choice questions. Designed with a charming anime-inspired book theme, it provides a fun and engaging way to learn.

## Features

*   **JSON Question Input:** Easily define your quiz questions using a flexible JSON format.
*   **Interactive Multiple Choice:** Users can select their answers with a simple click.
*   **Instant Answer Reveal:** Shows the correct answer and highlights the user's choice immediately after clicking "Show Answer".
*   **Book-like UI:** Navigate through questions like turning pages in a book, complete with animations.
*   **Question Navigation:** Jump directly to any question using the numbered buttons.
*   **Progress Tracking:** Visually indicates answered questions and the current question.
*   **Score Summary:** Displays the final score and a personalized message upon completion.
*   **Review Mode:** Review all questions and answers after finishing the quiz.
*   **Responsive Design:** Works well on various screen sizes.
*   **Anime Aesthetic:** Features pastel colors, gradients, floating decorations, and cute emojis for a fun visual experience.
*   **No Server Needed:** Runs entirely in the user's browser using a single HTML file.

## How to Use

1.  **Save the Code:** Copy the entire code block below and save it as an HTML file (e.g., `index.html`).
2.  **Open in Browser:** Open the `index.html` file in any modern web browser (Chrome, Firefox, Safari, Edge, etc.).
3.  **Input Questions:** Paste your quiz questions in the specified JSON format into the text area on the first page. A sample is provided for convenience.
4.  **Start Quiz:** Click the "📚 クイズを開始" (Start Quiz) button.
5.  **Answer Questions:**
    *   Select your chosen answer by clicking one of the options.
    *   Click the "💡 答えを表示" (Show Answer) button to see if you were correct.
    *   The correct answer will be revealed, and your choice will be marked.
6.  **Navigate:**
    *   Use the numbered buttons at the top to jump to any question.
    *   Use the "⬅️ 前のページ" (Previous Page) and "➡️ 次のページ" (Next Page) buttons to move sequentially.
    *   The "➡️ 次のページ" button appears after you've shown the answer for the current question (unless it's the last question).
7.  **Finish:** On the last question, the "➡️ 次のページ" button is replaced by "📊 結果を見る" (See Results). Click this to go to the results page.
8.  **Results Page:** View your score and a message. You can choose to "📚 最初のページに戻る" (Return to Start Page) or "📝 問題を見直す" (Review Questions).

## JSON Input Format

The quiz expects a JSON object containing a single key, `"questions"`, which holds an array of question objects. Each question object should have the following structure:

```json
{
  "questions": [
    {
      "question": "ここに問題文を書きます。",
      "choices": [
        { "option": 1, "text": "選択肢１" },
        { "option": 2, "text": "選択肢２" },
        { "option": 3, "text": "選択肢３" },
        { "option": 4, "text": "選択肢４" }
      ],
      "answer": 1 // 正解の選択肢の option 番号
    },
    // ... 次の問題
  ]
}
