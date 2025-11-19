# Contributing to AI Foundry workshop

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

 - [Code of Conduct](#coc)
 - [Issues and Bugs](#issue)
 - [Feature Requests](#feature)
 - [Submission Guidelines](#submit)

## <a name="coc"></a> Code of Conduct
Help us keep this project open and inclusive. Please read and follow our [Code of Conduct](https://opensource.microsoft.com/codeofconduct/).

## <a name="issue"></a> Found an Issue?
If you find a bug in the source code or a mistake in the documentation, you can help us by
[submitting an issue](#submit-issue) to the GitHub Repository. Even better, you can
[submit a Pull Request](#submit-pr) with a fix.

## <a name="feature"></a> Want a Feature?
You can *request* a new feature by [submitting an issue](#submit-issue) to the GitHub
Repository. If you would like to *implement* a new feature, please submit an issue with
a proposal for your work first, to be sure that we can use it.

* **Small Features** can be crafted and directly [submitted as a Pull Request](#submit-pr).

## <a name="submit"></a> Submission Guidelines

### <a name="submit-issue"></a> Submitting an Issue
Before you submit an issue, search the archive, maybe your question was already answered.

If your issue appears to be a bug, and hasn't been reported, open a new issue.
Help us to maximize the effort we can spend fixing issues and adding new
features, by not reporting duplicate issues.  Providing the following information will increase the
chances of your issue being dealt with quickly:

* **Overview of the Issue** - if an error is being thrown a non-minified stack trace helps
* **Version** - what version is affected (e.g. 0.1.2)
* **Motivation for or Use Case** - explain what are you trying to do and why the current behavior is a bug for you
* **Browsers and Operating System** - is this a problem with all browsers?
* **Reproduce the Error** - provide a live example or a unambiguous set of steps
* **Related Issues** - has a similar issue been reported before?
* **Suggest a Fix** - if you can't fix the bug yourself, perhaps you can point to what might be
  causing the problem (line of code or commit)

You can file new issues by providing the above information at the corresponding repository's issues link: https://github.com/[organization-name]/[repository-name]/issues/new].

### <a name="submit-pr"></a> Submitting a Pull Request (PR)

#### Step-by-Step Guide to Submit a Pull Request

**1. Verify Your Changes**

Before submitting, ensure your branch has the changes you want to contribute:

```bash
# Check the status of your local branch
git status

# Review your changes
git diff main

# View your commit history
git log --oneline -n 5
```

**2. Push Your Branch to GitHub**

If you haven't already pushed your branch, push it to your fork:

```bash
# Push your branch to your fork
git push origin your-branch-name

# Example: If your branch is named "feature/new-notebook"
git push origin feature/new-notebook
```

**3. Create the Pull Request on GitHub**

Once your branch is pushed, follow these steps to create a PR:

**Option A: Using GitHub Web Interface**

1. Navigate to your fork on GitHub: `https://github.com/YOUR-USERNAME/agentic-ai-lab`
2. You should see a banner saying "Your branch is ahead of `main`" with a **"Compare & pull request"** button
3. Click **"Compare & pull request"**
4. If you don't see the banner:
   - Click on the **"Pull requests"** tab
   - Click **"New pull request"**
   - Click **"compare across forks"**
   - Set the base repository to: `dhangerkapil/agentic-ai-lab` (or the original upstream repository)
   - Set the base branch to: `main`
   - Set the head repository to: `YOUR-USERNAME/agentic-ai-lab`
   - Set the compare branch to: `your-branch-name`

**Option B: Using GitHub CLI** (if you have `gh` installed)

```bash
# Create a PR directly from the command line
gh pr create --base main --head your-branch-name --title "Your PR Title" --body "Description of your changes"
```

**4. Fill Out the PR Template**

Provide a clear and descriptive PR description including:

* **Title**: A concise summary of your changes (e.g., "Add new embeddings tutorial notebook")
* **Description**: 
  - What changes did you make?
  - Why are these changes needed?
  - What issue does this resolve? (if applicable, use "Fixes #123")
  - Any additional context or screenshots

**Example PR Description:**

```markdown
## Summary
Added a new tutorial notebook for advanced embeddings techniques.

## Changes Made
- Created `chat-rag/4-advanced-embeddings.ipynb`
- Updated README.md to include the new notebook in the learning path
- Added sample data files in `chat-rag/data/`

## Testing
- Ran all cells in the notebook successfully
- Verified output matches expected results
- Tested with Azure AI Foundry deployment

Fixes #42
```

**5. Submit and Monitor Your PR**

* Click **"Create pull request"**
* The CLA bot will check if you need to sign the Contributor License Agreement
* If required, follow the instructions from the CLA bot to sign the agreement
* Wait for the maintainers to review your PR
* Respond to any feedback or requested changes

**6. Responding to Review Feedback**

If reviewers request changes:

```bash
# Make the requested changes in your local branch
# Edit files as needed

# Stage and commit your changes
git add .
git commit -m "Address review feedback: description of changes"

# Push the updates to your branch
git push origin your-branch-name
```

The PR will automatically update with your new commits.

**7. Keep Your Branch Updated** (if needed)

If the main branch has been updated since you created your PR:

```bash
# Add the upstream repository (only needed once)
git remote add upstream https://github.com/dhangerkapil/agentic-ai-lab.git

# Fetch the latest changes from upstream
git fetch upstream

# Merge the latest changes into your branch
git merge upstream/main

# Or rebase your branch onto the latest main
git rebase upstream/main

# Push the updated branch
git push origin your-branch-name
```

**Common PR Submission Scenarios:**

* **First-time contributor**: Don't forget to sign the CLA when prompted
* **Documentation changes**: Include screenshots if you're updating visual elements
* **New notebook**: Ensure all cells run successfully and outputs are cleared before committing
* **Bug fix**: Reference the issue number and include steps to reproduce the bug
* **New feature**: Consider opening an issue first to discuss the feature with maintainers

**Need Help?**

* Check the [GitHub Pull Request Documentation](https://docs.github.com/en/pull-requests)
* Review existing PRs in the repository for examples
* Open an issue if you're unsure about how to proceed

That's it! Thank you for your contribution! 🎉
