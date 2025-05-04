# Development Environment Setup (Step-by-Step Guide)

This guide will help you set up your local development environment to complete coding assignments successfully.

**Please follow each step carefully.**

## 1. Create a GitHub Account

### Steps:

1. Open your web browser and go to [https://github.com/](https://github.com/).
2. Click **Sign Up**.
3. Enter your:
   - Email address
   - Create a username
   - Create a password
4. Verify your email address.
5. Your GitHub account is ready.

**Tip**: Use your **Northeastern University email** for easier access to student benefits.

---

## 2. Apply for GitHub 🎓 Student Developer Pack

The GitHub Student Developer Pack gives you free access to many developer tools, including GitHub Copilot.

### Steps:

1. Open [https://education.github.com/pack](https://education.github.com/pack).
2. Click **Get Student Benefits**.
3. Log into GitHub if needed.
4. Choose **Student** as your role.
5. Submit proof of student status:
   - Use your **@northeastern.edu** email address when possible.
   - **Important**: If documentation is requested, upload a **current transcript** showing:
     - Your full name
     - The current semester
   - **Note**: **Student ID cards alone may not work** — they often do not show proof of current enrollment.
6. Wait for approval (usually within a day or two).

**Tip**: You can continue setting up your environment while waiting for approval.

---

## 3. Install Visual Studio Code (VS Code)

### Steps:

1. Visit [https://code.visualstudio.com/](https://code.visualstudio.com/).
2. Download and install the version for your operating system.
3. Accept default installation options.
4. Open **VS Code** to confirm it installed correctly.

---

## 4. Install Java (Amazon Corretto) ☕

We will use **Amazon Corretto 17** — a free, reliable distribution of Java.

### Steps:

1. Visit [https://docs.aws.amazon.com/corretto/latest/corretto-17-ug/downloads-list.html](https://docs.aws.amazon.com/corretto/latest/corretto-17-ug/downloads-list.html).
2. Download and install the version for your operating system.
3. Accept the license agreement.
4. Verify the installation by opening Terminal (Mac/Linux) or Command Prompt (Windows) and typing:

   ```bash
   java -version
   ```

   You should see output similar to:

   ```
   openjdk version "17.0.9" 2023-10-17
   OpenJDK Runtime Environment Corretto-17.0.9.8.1 (build 17.0.9+8-LTS)
   OpenJDK 64-Bit Server VM Corretto-17.0.9.8.1 (build 17.0.9+8-LTS, mixed mode, sharing)
   ```

---

## 5. Install Git 🔄

Git is essential for version control and submitting your assignments.

### Steps:

1. **Windows**:
   - Download Git from [https://git-scm.com/download/win](https://git-scm.com/download/win)
   - Run the installer, accepting default options
2. **macOS**:

   - If you have Homebrew: Open Terminal and type `brew install git`
   - Otherwise: Download from [https://git-scm.com/download/mac](https://git-scm.com/download/mac)

3. Verify installation by opening Terminal/Command Prompt and typing:

   ```bash
   git --version
   ```

4. Configure your Git identity:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your.email@northeastern.edu"
   ```

---

## 6. Configure VS Code for Java Development 🛠️

### Required Extensions:

1. Open VS Code
2. Click on the Extensions icon in the sidebar (or press `Ctrl+Shift+X`)
3. Install these essential extensions:
   - **Extension Pack for Java** by Microsoft
   - **GitHub Classroom** by GitHub
   - **Project Manager for Java** by Microsoft
   - **Maven for Java** by Microsoft
   - **Test Runner for Java** by Microsoft

### Configure Java Path:

1. Open VS Code Settings (`Ctrl+,` or `Cmd+,` on Mac)
2. Search for "java home"
3. Set the path to your Amazon Corretto JDK installation:
   - **Windows**: `C:\Program Files\Amazon Corretto\jdk17.x.x_x` (adjust version as needed)
   - **Mac**: `/Library/Java/JavaVirtualMachines/amazon-corretto-17.jdk/Contents/Home`
   - **Linux**: `/usr/lib/jvm/amazon-corretto-17` (may vary)

---

## 7. Set Up GitHub Copilot and GitHub Classroom 🤖🏫

For detailed instructions on setting up and using these tools:

- See 📄 **github-copilot-guide.md** - Complete setup and usage guide for GitHub Copilot
- See 📄 **github-classroom-guide.md** - Instructions for joining and submitting assignments

---

## 8. Basic Git Workflow for Assignments 📝

### Submit Your Work:

1. Make changes to your code ✏️
2. Stage your changes:
   ```bash
   git add .
   ```
3. Commit your changes:
   ```bash
   git commit -m "Meaningful description of your changes"
   ```
4. Push your changes to GitHub:
   ```bash
   git push origin main
   ```

**Note**: Always push your work before the ⏰ deadline!

---

## 9. Troubleshooting

### Java Not Found:

- Ensure Java is installed correctly
- Add Java to your PATH environment variable:
  - **Windows**: Search for "Environment Variables" > Edit System Variables > Add to PATH
  - **Mac/Linux**: Add `export PATH=$PATH:/path/to/java/bin` to your `.bash_profile` or `.zshrc`

### GitHub Authentication Issues:

- Try authenticating with a Personal Access Token (PAT)
- In GitHub: Settings > Developer Settings > Personal Access Tokens > Generate New Token
- Use this token when prompted for a password

### VS Code Extensions Not Working:

- Check that you have the correct version of Java installed
- Restart VS Code after installing extensions
- Try reinstalling the problematic extension

### Need Help?

If you encounter any issues not covered here, please:

1. Post in the course Teams channel
2. Check with classmates who may have solved the same issue
3. Attend office hours for personalized assistance

---

## 10. Additional Resources 📚

- [VS Code Java Tutorial](https://code.visualstudio.com/docs/java/java-tutorial) 📖
- [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf) 📋
- [GitHub Classroom Student Guide](https://github.com/jfiksel/github-classroom-for-students) 🎓
- [GitHub Copilot Documentation](https://docs.github.com/en/copilot) 🤖
