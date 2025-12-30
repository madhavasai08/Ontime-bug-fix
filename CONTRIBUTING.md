# Contributing to Ontime Bug Fix

Thank you for contributing to the Ontime project! This document provides guidelines for contributing bug fixes.

## Bug Fix Workflow

### 1. Identify the Bug

- Check if an issue already exists for the bug
- If not, create a new issue with:
  - Clear description of the bug
  - Steps to reproduce
  - Expected vs actual behavior
  - Environment details (OS, browser, versions)

### 2. Create a Branch

Always create a new branch for your bug fix:

```bash
git checkout -b fix/descriptive-bug-name
```

Branch naming conventions:
- `fix/` - for bug fixes
- `hotfix/` - for urgent production fixes
- `feature/` - for new features (if applicable)

### 3. Make Your Changes

- Keep changes focused on fixing the specific bug
- Follow the existing code style
- Add comments where necessary
- Update documentation if needed

### 4. Test Your Changes

Before committing:
- Test the specific bug fix
- Verify you haven't broken existing functionality
- Test edge cases
- Run any existing test suites

### 5. Commit Your Changes

Write clear, descriptive commit messages:

```bash
git add .
git commit -m "Fix: Brief description of the bug fix

- Detailed explanation of what was changed
- Why the change was necessary
- Any side effects or dependencies"
```

Good commit message examples:
- `Fix: Null reference exception in user login`
- `Fix: Incorrect date format in report generation`
- `Hotfix: Memory leak in background task processing`

### 6. Push and Create Pull Request

```bash
git push origin fix/descriptive-bug-name
```

Then create a Pull Request on GitHub with:
- Reference to the issue number (e.g., "Fixes #123")
- Summary of changes
- Testing performed
- Screenshots (if UI changes)

## Code Review Process

1. All changes require review before merging
2. Address reviewer feedback promptly
3. Keep the PR focused and small when possible
4. Be open to suggestions and improvements

## Need Help?

If you're stuck or have questions:
- Open an issue for discussion
- Tag relevant team members
- Check existing documentation

## Code of Conduct

- Be respectful and professional
- Provide constructive feedback
- Help others learn and grow
- Focus on the code, not the person

Thank you for helping improve Ontime!
