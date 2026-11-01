Step 1: Install Git and Verify
If you haven't installed Git yet, download and install it from git-scm.com.
Open your command prompt or terminal and run the verification command:

Bash
git --version
Verification: You should see an output displaying your installed Git version (e.g., git version 2.x.x).

Step 2: Open the Terminal in the Project Folder
Create a new folder on your computer for this project (for example, name it git-assignment).

Open Visual Studio Code, go to File > Open Folder, and select your new project folder.

Open the integrated terminal in VS Code by pressing Ctrl + ` (or going to Terminal > New Terminal).

Step 3: Initialize Git
In your terminal, run the following command to initialize an empty Git repository in your project folder:

Bash
git init
Verification: You should see a message saying Initialized empty Git repository in .../.git/. (If you don't see it, make sure hidden files are visible to confirm the .git folder was created).

Step 4: Configure Your Git Username and Email
Set up your global or local identity so your commits are correctly attributed to you. Run these commands with your own name and email:

Bash
git config --global user.name "Atim Akhtar"
git config --global user.email "your-email@example.com"
Verification: You can verify your settings by running git config --list.

Step 5: Create an HTML File
Create your first file inside the project directory.

In VS Code, create a new file named index.html.

Add some basic HTML boilerplate structure (for example, a simple heading):

HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Git Assignment</title>
</head>
<body>
    <h1>Hello World</h1>
</body>
</html>
Step 6: Use git status, git add, and git commit (Making 3 Meaningful Commits)
To fulfill the requirement of at least 3 meaningful commits, you should make incremental changes to your project, staging and committing them separately.

Commit 1: Initial HTML Structure
Check the status of your repository:

Bash
git status
(Verification: index.html will appear in red as an untracked file.)

Stage the file:

Bash
git add index.html
Commit the file with a meaningful message:

Bash
git commit -m "chore: add initial HTML boilerplate structure"
Commit 2: Add a Paragraph or Navigation Section
Open index.html and add a new element, such as a paragraph or a footer:

HTML
<p>Welcome to my first version-controlled web project.</p>
Check status, add, and commit:

Bash
git status
git add index.html
git commit -m "feat: add introductory paragraph to homepage"
Commit 3: Add Styling or Metadata
Add a meta tag or minor style update inside index.html:

HTML
<meta name="viewport" content="width=device-width, initial-scale=1.0">
Check status, add, and commit:

Bash
git status
git add index.html
git commit -m "style: add viewport meta tag for responsiveness"
Step 7: Verify Your Commit History for Submission
To capture the required screenshots for your submission, verify your commit history by running:

Bash
git log --oneline
Verification: You should see a list of your 3 commits with their respective hash IDs and commit messages.

Required Submissions:
Screenshot 1: Take a screenshot of your project folder open in VS Code (showing the file structure and terminal).

Screenshot 2: Take a screenshot of your terminal window showing the output of git log --oneline (displaying all 3 meaningful commits).