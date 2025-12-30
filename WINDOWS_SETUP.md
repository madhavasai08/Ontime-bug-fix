# Quick Start Guide for Windows Users

This guide is specifically for pushing your Ontime code from:
**`D:\Ontime\New patch fix code 12302025\site\wwwroot`**

## Step-by-Step Instructions

### Step 1: Install Git (if not already installed)

1. Download Git from: https://git-scm.com/download/win
2. Run the installer with default settings
3. Verify installation by opening Command Prompt and typing:
   ```
   git --version
   ```

### Step 2: Configure Git (First Time Only)

Open Command Prompt or Git Bash and run:
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### Step 3: Choose Your Approach

#### **OPTION A: Clone Repository Then Copy Files (EASIEST)**

1. Open Command Prompt (Win + R, type `cmd`, press Enter)

2. Navigate to a working directory:
   ```cmd
   cd D:\Ontime
   ```

3. Clone this repository:
   ```cmd
   git clone https://github.com/madhavasai08/Ontime-bug-fix.git
   ```

4. Copy your code files:
   ```cmd
   cd Ontime-bug-fix
   xcopy "..\New patch fix code 12302025\site\wwwroot\*" . /E /H /C /I
   ```
   
   **OR** manually copy all files from:
   - From: `D:\Ontime\New patch fix code 12302025\site\wwwroot`
   - To: `D:\Ontime\Ontime-bug-fix`

5. Add and commit files:
   ```cmd
   git add .
   git commit -m "Add Ontime codebase from wwwroot"
   ```

6. Push to GitHub:
   ```cmd
   git push origin main
   ```

#### **OPTION B: Initialize Git in Your Existing Directory**

1. Open Command Prompt

2. Navigate to your code directory:
   ```cmd
   cd "D:\Ontime\New patch fix code 12302025\site\wwwroot"
   ```

3. Initialize Git:
   ```cmd
   git init
   ```

4. Add remote:
   ```cmd
   git remote add origin https://github.com/madhavasai08/Ontime-bug-fix.git
   ```

5. Pull README and setup files:
   ```cmd
   git pull origin main --allow-unrelated-histories
   ```

6. Add all your files:
   ```cmd
   git add .
   ```

7. Commit:
   ```cmd
   git commit -m "Add Ontime codebase from wwwroot"
   ```

8. Push:
   ```cmd
   git push -u origin main
   ```

### Step 4: Verify Your Code is on GitHub

1. Go to: https://github.com/madhavasai08/Ontime-bug-fix
2. You should see all your code files listed

## Working on Bug Fixes

After your initial push, use this workflow:

1. **Create a bug fix branch:**
   ```cmd
   git checkout -b fix/bug-description
   ```

2. **Make your changes** in your code editor

3. **Check what changed:**
   ```cmd
   git status
   git diff
   ```

4. **Commit changes:**
   ```cmd
   git add .
   git commit -m "Fix: description of what was fixed"
   ```

5. **Push branch:**
   ```cmd
   git push origin fix/bug-description
   ```

6. **Create Pull Request** on GitHub website

## Troubleshooting

### Authentication Issues

If asked for credentials, you may need a Personal Access Token:
1. Go to GitHub → Settings → Developer settings → Personal access tokens
2. Generate new token with `repo` permissions
3. Use token as password when prompted

### Large Files

If you have large files (>100MB):
- Add them to `.gitignore` before committing
- Or use Git LFS: https://git-lfs.github.com/

### Merge Conflicts

If you get merge conflicts:
```cmd
git pull origin main
# Resolve conflicts in your editor
git add .
git commit -m "Resolve merge conflicts"
git push
```

## Quick Commands Reference

```cmd
# Check status
git status

# See changes
git diff

# Undo changes to a file
git checkout -- filename

# Update from GitHub
git pull

# See commit history
git log --oneline
```

## Need Help?

- Git Documentation: https://git-scm.com/doc
- GitHub Guides: https://guides.github.com/
- Contact: [Add your contact information]
