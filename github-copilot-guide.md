# GitHub Copilot Setup & Usage Guide

## What is GitHub Copilot?

GitHub Copilot is an AI pair programmer that helps you write code faster and with less work. It draws context from comments and code to suggest individual lines and whole functions instantly. GitHub Copilot is powered by OpenAI's advanced models and is trained on billions of lines of public code.

## Benefits for Students

- **Accelerate Learning**: Learn coding patterns and techniques faster
- **Reduce Boilerplate**: Spend less time writing repetitive code
- **Focus on Logic**: Concentrate on solving problems rather than syntax
- **Explore Alternatives**: See different approaches to the same problem
- **Improve Code Quality**: Get suggestions for more efficient code

---

## Setup Instructions

### Prerequisites

- GitHub account (created in Step 1 of main setup guide)
- GitHub Student Developer Pack approved (Step 2 of main setup guide)
- Visual Studio Code installed (Step 3 of main setup guide)

### Installation Steps

1. **Open VS Code**
2. **Access Extensions**

   - Click the Extensions icon in the Activity Bar on the side of the window
   - OR press `Ctrl+Shift+X` (Windows/Linux) or `Cmd+Shift+X` (Mac)

3. **Install GitHub Copilot**

   - Search for "GitHub Copilot"
   - Click **Install** on "GitHub Copilot" by GitHub

4. **Sign In to GitHub**

   - After installation, you'll be prompted to sign in to GitHub
   - Follow the authentication flow in your browser
   - Make sure to sign in with the same GitHub account that has the Student Developer Pack

5. **Verify Activation**
   - Look for the GitHub Copilot icon in the status bar at the bottom of VS Code
   - It should be active and not showing any warnings

---

## Using GitHub Copilot

### Basic Usage

1. **Start Typing Code**

   - As you type, Copilot will suggest code completions in gray text
   - Press `Tab` to accept a suggestion
   - Press `Esc` to dismiss a suggestion
   - Continue typing to see different suggestions

2. **Generate from Comments**

   - Write a comment describing what you want to do
   - Press Enter to start a new line
   - Copilot will suggest code that implements your comment

   Example:

   ```java
   // Find the maximum value in an array of integers
   ```

3. **Complete Function Bodies**

   - Type a function signature and open curly brace
   - Copilot will suggest the entire function implementation

   Example:

   ```java
   public int factorial(int n) {
       // Copilot will suggest the factorial implementation
   }
   ```

### Advanced Features

#### GitHub Copilot Chat (Agent Mode)

Copilot Chat is a more interactive way to use AI assistance for coding tasks.

1. **Access Copilot Chat**

   - Press `Ctrl+I` (Windows/Linux) or `Cmd+I` (Mac)
   - OR click the Copilot Chat icon in the sidebar

2. **Ask Questions or Request Code**

   - "Write a function to convert Celsius to Fahrenheit"
   - "How do I read a CSV file in Java?"
   - "Explain how this algorithm works"

3. **Get Multi-file Assistance**
   - "Refactor this class to use the Builder pattern"
   - "Find and fix bugs in my code"
   - "Help me implement a feature across multiple files"

#### Keyboard Shortcuts

| Action                    | Windows/Linux | Mac        |
| ------------------------- | ------------- | ---------- |
| Accept suggestion         | `Tab`         | `Tab`      |
| Dismiss suggestion        | `Esc`         | `Esc`      |
| Show next suggestion      | `Alt+]`       | `Option+]` |
| Show previous suggestion  | `Alt+[`       | `Option+[` |
| Open Copilot Chat         | `Ctrl+I`      | `Cmd+I`    |
| Trigger inline suggestion | `Alt+\`       | `Option+\` |

---

## Best Practices for INFO5001

### Do's

- **Use Copilot to Learn**: Analyze its suggestions to understand coding patterns
- **Review All Code**: Always check and understand the code before submitting
- **Write Good Comments**: Clear comments lead to better suggestions
- **Use Copilot for Boilerplate**: Let it handle repetitive code patterns
- **Ask for Explanations**: Use Chat to understand concepts and techniques

### Don'ts

- **Don't Submit Code You Don't Understand**: Make sure you can explain your code
- **Don't Rely Exclusively on Copilot**: It's a tool, not a replacement for learning
- **Don't Skip Testing**: Always test the generated code for correctness
- **Don't Accept Every Suggestion**: Be critical and selective
- **Don't Use for Exams**: Unless explicitly permitted by the instructor

---

## Ethical Considerations

- **Academic Integrity**: Using Copilot is allowed for assignments in this course, but you must understand the code you submit
- **Attribution**: If Copilot helps you implement a complex algorithm, noting this in comments is good practice
- **Learning Goals**: Remember that the goal is to learn programming, with Copilot as a helpful assistant

---

## Troubleshooting

### Common Issues and Solutions

- **Copilot Not Activating**:

  - Verify your GitHub account has the Student Developer Pack
  - Try signing out and back in to GitHub in VS Code
  - Check your internet connection

- **Poor Suggestions**:

  - Provide more context in your code or comments
  - Try writing more specific comments
  - Break complex tasks into smaller parts

- **High Latency**:
  - Check your internet connection
  - Wait a moment before dismissing suggestions
  - Restart VS Code if the issue persists

---

## Additional Resources

- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [GitHub Copilot for Students](https://github.blog/2022-09-08-github-copilot-now-available-for-teachers/)
- [VS Code & GitHub Copilot](https://code.visualstudio.com/docs/editor/github-copilot)
- [Effective Prompting for Copilot](https://github.blog/2023-06-20-how-to-write-better-prompts-for-github-copilot/)

---

_Remember, GitHub Copilot is a tool to enhance your learning journey, not replace it. Use it wisely and ethically!_
