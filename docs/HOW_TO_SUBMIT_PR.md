# How to Submit a Pull Request

This guide provides a quick reference for submitting pull requests to the agentic-ai-lab repository.

## Quick Steps

### 1️⃣ Push Your Branch

```bash
# Check your current branch
git branch

# Push your branch to your fork
git push origin your-branch-name
```

### 2️⃣ Open Pull Request on GitHub

1. Go to your fork: `https://github.com/YOUR-USERNAME/agentic-ai-lab`
2. Click the **"Compare & pull request"** button (appears after pushing)
3. Or navigate to: **Pull requests** → **New pull request** → **compare across forks**

### 3️⃣ Configure PR Settings

**Base repository:** `dhangerkapil/agentic-ai-lab` (upstream)  
**Base branch:** `main`  
**Head repository:** `YOUR-USERNAME/agentic-ai-lab` (your fork)  
**Compare branch:** `your-branch-name`

### 4️⃣ Write PR Description

```markdown
## Summary
Brief description of what this PR does

## Changes Made
- List of changes
- Another change
- And another

## Testing
How you tested these changes

Fixes #issue-number (if applicable)
```

### 5️⃣ Submit & Sign CLA

- Click **"Create pull request"**
- Sign the Contributor License Agreement (CLA) if prompted
- Wait for review from maintainers

---

## Using GitHub CLI (Optional)

If you have `gh` CLI installed:

```bash
# Create PR from command line
gh pr create --base main --title "Your PR title" --body "Your description"

# Check PR status
gh pr status

# View PR in browser
gh pr view --web
```

---

## Updating Your PR After Feedback

```bash
# Make requested changes
# Edit files as needed

# Commit and push
git add .
git commit -m "Address review feedback"
git push origin your-branch-name
```

Your PR will automatically update! ✨

---

## Common Issues & Solutions

### Issue: "No changes detected"
**Solution:** Make sure you've committed your changes before pushing:
```bash
git add .
git commit -m "Your commit message"
git push origin your-branch-name
```

### Issue: "Conflicts with base branch"
**Solution:** Update your branch with the latest changes:
```bash
git fetch upstream
git merge upstream/main
# Resolve conflicts if any
git push origin your-branch-name
```

### Issue: "CLA check failed"
**Solution:** Click the CLA bot link in your PR and follow the instructions to sign the Contributor License Agreement.

---

## Best Practices

✅ **Do:**
- Write clear, descriptive PR titles
- Include detailed description of changes
- Reference related issues using `Fixes #123`
- Test your changes before submitting
- Respond promptly to reviewer feedback
- Keep commits focused and logical

❌ **Don't:**
- Submit large PRs that change many unrelated things
- Include temporary/test files
- Push directly to main branch
- Force-push after PR is created (unless requested by maintainers)

---

## Need More Help?

📖 **Full Guide:** See [CONTRIBUTING.md](../CONTRIBUTING.md) for detailed instructions  
🐛 **Issues:** [Open an issue](https://github.com/dhangerkapil/agentic-ai-lab/issues/new) if you need help  
💬 **Questions:** Check existing [Pull Requests](https://github.com/dhangerkapil/agentic-ai-lab/pulls) for examples

---

Happy Contributing! 🎉
