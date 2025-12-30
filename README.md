# Ontime-bug-fix

A repository for tracking and fixing bugs in the Ontime codebase.

## Getting Started

### Prerequisites
- Git installed on your local machine ([Download Git](https://git-scm.com/downloads))
- GitHub account
- Your codebase at: `D:\Ontime\New patch fix code 12302025\site\wwwroot`

### Initial Setup - Option 1: Copy Files to Cloned Repository (Recommended)

1. **Clone this repository** to your local machine:
   ```bash
   # Open Git Bash or Command Prompt
   cd D:\Ontime
   git clone https://github.com/madhavasai08/Ontime-bug-fix.git
   cd Ontime-bug-fix
   ```

2. **Copy your code** from the wwwroot directory:
   ```bash
   # Windows Command Prompt:
   xcopy "D:\Ontime\New patch fix code 12302025\site\wwwroot\*" . /E /H /C /I
   
   # Or use Windows Explorer to copy all files from:
   # D:\Ontime\New patch fix code 12302025\site\wwwroot
   # To: D:\Ontime\Ontime-bug-fix
   ```

3. **Stage your changes**:
   ```bash
   git add .
   ```

4. **Commit your changes**:
   ```bash
   git commit -m "Add initial Ontime codebase from wwwroot"
   ```

5. **Push to GitHub**:
   ```bash
   git push origin main
   ```

### Initial Setup - Option 2: Initialize Git in Existing Directory

If you prefer to work directly in your existing directory:

1. **Navigate to your code directory**:
   ```bash
   cd "D:\Ontime\New patch fix code 12302025\site\wwwroot"
   ```

2. **Initialize Git** (if not already initialized):
   ```bash
   git init
   ```

3. **Add the remote repository**:
   ```bash
   git remote add origin https://github.com/madhavasai08/Ontime-bug-fix.git
   ```

4. **Pull the latest changes** (to get README and other setup files):
   ```bash
   git pull origin main --allow-unrelated-histories
   ```

5. **Stage all your files**:
   ```bash
   git add .
   ```

6. **Commit your changes**:
   ```bash
   git commit -m "Add initial Ontime codebase from wwwroot"
   ```

7. **Push to GitHub**:
   ```bash
   git push -u origin main
   ```

### Working on Bug Fixes

1. **Create a new branch** for each bug fix:
   ```bash
   git checkout -b fix/bug-description
   ```

2. **Make your changes** and test them thoroughly

3. **Commit your changes**:
   ```bash
   git add .
   git commit -m "Fix: description of the bug fix"
   ```

4. **Push your branch**:
   ```bash
   git push origin fix/bug-description
   ```

5. **Create a Pull Request** on GitHub for review

## Repository Structure

```
Ontime-bug-fix/
├── README.md           # This file
├── CONTRIBUTING.md     # Contribution guidelines
├── .gitignore         # Git ignore patterns
├── docs/              # Documentation
├── src/               # Source code (add your code here)
└── tests/             # Test files
```

## Bug Tracking

Please use GitHub Issues to track bugs:
1. Go to the Issues tab
2. Click "New Issue"
3. Provide a clear title and description
4. Add appropriate labels

## Need Help?

- [Git Documentation](https://git-scm.com/doc)
- [GitHub Guides](https://guides.github.com/)
- [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/)

## License

Add your license information here.