# GitHub Repository Lifecycle Guide

## Important: Preserving Your Course Work

GitHub Classroom repositories created for this course are **temporary** and will be **deleted** after the course ends. To keep your work for your portfolio or future reference, you need to transfer it to your personal GitHub account.

## Why Should You Keep Your Work?

- **Portfolio Development**: Showcase your coding projects to potential employers
- **Reference Material**: Revisit your solutions for future coursework or projects
- **Professional Growth**: Track your progression as a developer
- **Knowledge Base**: Build your personal library of coding patterns and solutions

---

## When Will Repositories Be Deleted?

- Course repositories are typically maintained for **3 months** after the course end date
- After this period, **all content will be permanently deleted** without further notice
- This applies to all assignments, projects, and other repositories created via GitHub Classroom

---

## How to Preserve Your Work

There are three main methods to preserve your work. Choose the approach that works best for you:

### Method 1: Create a New Repository (Recommended)

This method preserves your entire project history and structure:

1. **Create a new personal repository**:

   - Go to [GitHub](https://github.com) and log in
   - Click the "+" icon in the top-right corner and select "New repository"
   - Name your repository (e.g., "INFO5001-Project-Portfolio")
   - Choose "Public" or "Private" visibility
   - Do NOT initialize with README, .gitignore, or license
   - Click "Create repository"

2. **Clone your classroom repository locally** (if you haven't already):

   ```bash
   git clone https://github.com/classroom-org/your-assignment-repo.git
   cd your-assignment-repo
   ```

3. **Change the remote URL to your new repository**:

   ```bash
   git remote set-url origin https://github.com/YOUR-USERNAME/YOUR-NEW-REPO.git
   ```

4. **Push everything to your new repository**:
   ```bash
   git push -u origin main
   ```

### Method 2: Copy Selected Files

If you only want to preserve specific files or the latest version:

1. **Create a new repository** as described in Method 1

2. **Download your classroom repository as a ZIP file**:

   - Go to your classroom repository on GitHub
   - Click the green "Code" button
   - Select "Download ZIP"

3. **Unzip and copy the files** to your local computer

4. **Clone your new personal repository**:

   ```bash
   git clone https://github.com/YOUR-USERNAME/YOUR-NEW-REPO.git
   cd YOUR-NEW-REPO
   ```

5. **Copy your files** into this new repository directory

6. **Commit and push your files**:
   ```bash
   git add .
   git commit -m "Preserved files from INFO5001 course"
   git push origin main
   ```

---

## Preserving Multiple Repositories

If you have multiple assignments or projects to preserve:

### Option 1: Create Separate Repositories

- Create individual repositories for each project
- Follow Method 1 or 2 above for each repository
- This keeps projects distinct and easily identifiable

### Option 2: Create One Portfolio Repository with Subfolders

1. **Create one main repository** (e.g., "INFO5001-Portfolio")

2. **Create a folder structure** in your new repository:

   ```
   INFO5001-Portfolio/
   ├── Assignment1/
   ├── Assignment2/
   ├── Project1/
   └── Project2/
   ```

3. **Copy files** from each classroom repository into the appropriate folders

4. **Commit and push** each addition separately:

   ```bash
   git add Assignment1
   git commit -m "Add Assignment 1 to portfolio"
   git push

   git add Assignment2
   git commit -m "Add Assignment 2 to portfolio"
   git push
   ```

---

## Additional Tips

1. **Clean up before preserving**:

   - Remove unnecessary files (compiled code, temporary files)
   - Update README files to explain the project context

2. **Add documentation**:

   - Create a brief description of what you learned
   - Note any interesting challenges you overcame
   - Include screenshots of the application if applicable

3. **Update visibility settings** if needed:

   - Private repositories are good for sensitive or incomplete work
   - Public repositories are better for portfolios you want to share

4. **Add a license** if you plan to make your code public:
   - Go to your repository on GitHub
   - Click "Add file" > "Create new file"
   - Name it "LICENSE"
   - Click "Choose a license template" and select one (MIT is common for personal projects)

---

## Troubleshooting Common Issues

### Authentication Errors

If you see "Authentication failed" when pushing to your new repository:

- Ensure you're using a personal access token or SSH key
- Create a personal access token at GitHub > Settings > Developer Settings > Personal Access Tokens
- Use this token when prompted for a password

### "Repository not found" Error

- Double-check the URL of your new repository
- Make sure you've created the repository on GitHub
- Verify that you have the correct username in the URL

### Unable to Push ("rejected" errors)

- Try pulling changes first: `git pull --rebase origin main`
- Force push if needed (use with caution): `git push -f origin main`

---

_Remember: It's YOUR responsibility to preserve your work before the deletion deadline. Set a reminder to complete this process before the 3-month post-course period ends._
