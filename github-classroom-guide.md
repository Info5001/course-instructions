# GitHub Classroom Guide for INFO5001 🏫👨‍💻

## What is GitHub Classroom? 🎓

GitHub Classroom is a teaching tool that allows instructors to distribute coding assignments, provide feedback, and manage submissions through GitHub. It automates repository creation, access control, and provides a streamlined workflow for programming courses.

## Benefits of GitHub Classroom 🌟

- **Automated Setup** ⚙️: Easily access assignments through a single link
- **Real-world Skills** 💼: Learn Git and GitHub, the same tools used by professional developers
- **Immediate Feedback** 💬: See build errors and instructor comments directly in code
- **Portfolio Building** 📂: Build a collection of projects visible to potential employers
- **Collaboration** 👥: Learn to work with others using professional tools

---

## Getting Started with GitHub Classroom 🚀

### Prerequisites

- ✅ GitHub account (created in Step 1 of main setup guide)
- ✅ Git installed on your computer (Step 5 of main setup guide)
- ✅ VS Code with GitHub Classroom extension installed (Step 6 of main setup guide)

---

## Accepting Assignments 📝

### Steps for Accepting Your First Assignment

1. **Access the Invitation Link** 📧

   - You'll receive assignment links via Canvas announcements or email
   - Click the link to open the GitHub Classroom assignment page

2. **Join the Classroom** 🏛️

   - If this is your first assignment, you'll be asked to join the classroom
   - Select your name from the roster to link your GitHub account

   ![Join Classroom](https://docs.github.com/assets/cb-77734/mw-1440/images/help/classroom/assignments-click-join-roster.webp)

3. **Accept the Assignment** ✅

   - Click the "Accept this assignment" button
   - GitHub Classroom will create a personal copy (repository) of the assignment for you

   ![Accept Assignment](https://docs.github.com/assets/cb-150109/mw-1440/images/help/classroom/assignments-accept-button.webp)

4. **Wait for Repository Creation** ⏳

   - GitHub will automatically create your assignment repository
   - When ready, you'll see a link to your new repository

   ![Repository Created](https://docs.github.com/assets/cb-106934/mw-1440/images/help/classroom/assignment-accepted-link.webp)

5. **Open the Repository** 🔗
   - Click on the link to open your personal assignment repository
   - This is where you'll work on your assignment

---

## Working on Assignments Locally 💻

### Cloning Your Assignment Repository

1. **Copy Repository URL** 📋

   - On your assignment repository page, click the green "Code" button
   - Copy the HTTPS URL

   ![Clone URL](https://docs.github.com/assets/cb-127534/mw-1440/images/help/repository/code-button.webp)

2. **Clone in VS Code** 🧩

   - Open VS Code
   - Press `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac) to open Command Palette
   - Type "Git: Clone" and select it
   - Paste the repository URL and select a local folder to store the project

   OR

   **Clone using Terminal** 💻

   ```bash
   git clone https://github.com/classroom-org/assignment-your-username.git
   cd assignment-your-username
   code .  # Opens the project in VS Code
   ```

3. **Open the Project** 📂
   - VS Code will open the cloned repository
   - You can now see all the assignment files and start working

---

## Completing and Submitting Assignments 📤

### The Git Workflow for Assignments

1. **Make Changes to Code** ✏️

   - Implement your solution in the provided files
   - Create new files if needed

2. **Save Your Changes** 💾

   - Save your files in VS Code (`Ctrl+S` or `Cmd+S`)

3. **Stage Your Changes** ➕

   - In VS Code, open the Source Control panel (click the branch icon in the sidebar)
   - Click the "+" next to modified files to stage them

   OR using Terminal:

   ```bash
   git add .  # Stages all changes
   ```

4. **Commit Your Changes** 📝

   - Write a meaningful commit message (e.g., "Implemented factorial function")
   - Click the checkmark icon to commit

   OR using Terminal:

   ```bash
   git commit -m "Implemented factorial function"
   ```

5. **Push to GitHub** 🚀

   - Click the "..." in the Source Control panel and select "Push"
   - OR click on the sync icon in the status bar

   OR using Terminal:

   ```bash
   git push origin main
   ```

6. **Verify Submission** ✅
   - Visit your GitHub repository page to confirm your changes are visible
   - Check for any automated feedback or tests that have run

---

## Best Practices for GitHub Classroom 🌟

### Do's ✅

- **Commit Frequently** 🕒: Make small, frequent commits with clear messages
- **Keep Your Repository Clean** 🧹: Don't commit unnecessary files like compiled binaries
- **Read Assignment Instructions Carefully** 📖: Check the README.md file for requirements
- **Start Early** ⏰: Don't wait until the last minute to begin assignments
- **Ask for Help** 🙋‍♂️: Use class discussions to ask questions if you're stuck

### Don'ts ❌

- **Don't Share Your Repository** 🚫: Your assignment repo should remain private
- **Don't Wait Until the Deadline** ⏱️: Push your work regularly, not just at the last minute
- **Don't Ignore Automated Feedback** 🤖: Check for automated tests and fix failures
- **Don't Commit Credentials** 🔑: Never push API keys or passwords to GitHub
- **Don't Make a Single Giant Commit** 📦: Break your work into logical, smaller commits

---

## Working with GitHub Classroom in VS Code 🧰

### Using the GitHub Classroom Extension

1. **Open VS Code** 💻

2. **Access Your Assignments** 📚

   - Click on the GitHub Classroom icon in the Activity Bar
   - You'll see a list of your assignments

   ![GitHub Classroom Extension](https://github.com/github/github-vscode-theme/raw/master/screenshots/preview.png)

3. **Clone an Assignment** 📥

   - Click on an assignment in the list
   - Select "Clone assignment"
   - Choose a location on your computer

4. **Submit Assignment** 📤
   - After making changes, use the Source Control panel to commit and push
   - The extension will show submission status

---

## Advanced GitHub Features for Students 🔧

### GitHub Issues

- **Track Tasks** 📋: Create issues for features you need to implement
- **Ask Questions** ❓: If enabled, use issues to ask specific questions about the assignment

### Pull Requests

- **Self-Review** 🔍: Create pull requests to review your own code
- **Get Feedback** 💬: Instructors may use pull requests to provide line-by-line feedback

### GitHub Actions

- **Automated Tests** 🧪: Some assignments may include automatic tests
- **Check Status** ✓: Look for the green checkmark that indicates your code passes tests

---

## Troubleshooting GitHub Classroom 🔍

### Common Issues and Solutions

- **Authentication Failed** 🔒:

  - Use a personal access token instead of password
  - Create one at GitHub > Settings > Developer Settings > Personal Access Tokens

- **Cannot Push Changes** ⚠️:

  - Ensure you've committed your changes first
  - Check if you have write access to the repository
  - Try `git pull` first to sync with remote changes

- **Assignment Link Not Working** 🔗:

  - Make sure you're logged into GitHub
  - Check if the assignment deadline has passed
  - Contact your instructor for help

- **Repository Not Showing in VS Code** 🔎:
  - Try refreshing the GitHub Classroom extension
  - Clone the repository manually using the terminal

---

## Additional Resources 📚

- [GitHub Classroom Student Guide](https://github.com/jfiksel/github-classroom-for-students) 📖
- [GitHub Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf) 📄
- [GitHub Skills](https://skills.github.com/) 🎮
- [Pro Git Book](https://git-scm.com/book/en/v2) (free online) 📗
- [Markdown Guide](https://www.markdownguide.org/) for README files 📝

---

_Remember: GitHub is not just a tool for this class—it's an industry-standard platform that will benefit your career. Learning it well now will pay dividends later!_ 💯
