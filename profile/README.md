# Agentic Education Practitioners Association at Agentic-ED.org

The Agentic Education Practitioners Association consists of multiple Guilds. Our Guilds build and freely share **open-source AI agents and agent skills under the MIT License**. We also host educational programs where practitioners can share what they learn from both building skills and agents and using them in their respeective practices.

[Explore the Guilds](https://agentic-ed.org/Guilds) · [Browse the repositories](https://github.com/orgs/Agentic-ED/repositories) · [Sign up](https://agentic-ed.org/signup)

## Find an asset you can use

We recommend that you start with the work you want to do. An **agent skill** gives an AI environment instructions for a particular task and may include scripts, examples, or reference files. An **agent** uses instructions and tools to carry out a workflow. Download the skill or agent from its repository and check its README for setup, dependencies, and compatibility with your environment, such as Claude, Gemini, Codex, and the like. For skills, you most likely can simply share the skill folder URL with the agent. 


## Find your Guild

Each Guild focuses on one area of practice and takes its name from a group of animals. The animal is also the Guild’s AI steward. Members choose priorities, the steward helps review contributions, and Human leaders of the Guild approve releases. That's a high level take on it, but there are mechanics associated with AI budgets, membership voting, and project prioritizations. 

| If you work on… | Explore | Steward |
|---|---|---|
| Community and events | The Ostentation, the home Guild every member joins | Peacock |
| Curriculum development | The Colony | Beaver |
| Customer education | The Exaltation | Lark |
| Training | The Romp | Otter |
| Certification | The Parliament | Owl |

[See all Guilds and their repositories](https://agentic-ed.org/Guilds)

## Learn and contribute

Start with the [Guild repository](https://github.com/orgs/Agentic-ED/repositories) that owns the agent or skill you want to improve, enhance, or optimize.

[Find a Guild to contribute to](https://agentic-ed.org/Guilds)

Read its README and any `CONTRIBUTING.md` instructions. Open an issue to report a problem or propose an enhancement. Open a pull request when you have changes ready for review.

### File an issue

In the Guild repository, select **Issues** and search for related work. Add your example to an existing issue or select **New issue** and choose a template if offered. Use examples you have permission to share publicly.

- **Bug report example — Curriculum review skill skips objectives in tables.** Include a sample lesson with one objective in a paragraph and another in a table. Name the skill and AI environment you tested. Describe which objectives you expected the review to cover and which it actually covered.
- **Enhancement example — Add a worked example to the curriculum review skill.** Describe the task and what would help. For example, “I’d like a sample lesson, a prompt I can try, and a sample review so I can compare the result with my own.” If you plan to contribute the example, mention that in the issue.

### Example 1 — Fix a skill using a local clone

1. **Fork the repository.** Sign in to GitHub. On the Guild repository page, select **Fork → Create fork** to make a copy under your account.
2. **Clone your fork and create a branch.** On your fork, copy the HTTPS URL from the **Code** menu. Substitute that URL and the repository directory name below.

   ```bash
   git clone https://github.com/YOUR-USERNAME/REPOSITORY.git
   cd REPOSITORY
   git switch -c fix/table-objectives
   ```

3. **Edit and test.** For the table issue above, run the sample lesson with the current skill. Update the instructions, then run the same lesson again. Check whether the review covers both objectives. Run any checks listed in the repository.
4. **Commit and push.** Substitute the paths of the files you edited. Review the staged changes before committing.

   ```bash
   git status
   git add path/to/changed-file
   git diff --staged
   git commit -m "Include objectives from tables in curriculum reviews"
   git push -u origin fix/table-objectives
   ```

5. **Open a pull request.** On GitHub, select **Compare & pull request**. Set the **base** to the original Guild repository and its target branch. Set the **head** to your fork and `fix/table-objectives`. Link the issue, explain the fix, and include your before-and-after results. Review the files and select **Create pull request**.

### Example 2 — Add a worked example using VS Code in your browser

1. **Open your fork in VS Code.** Sign in to GitHub, open the Guild repository, and select **Fork → Create fork**, or open your existing fork. While viewing your fork, press the period key (`.`) to open VS Code for the Web.
2. **Create a branch.** Select the current branch name in the lower-left corner, enter `add-curriculum-review-example`, and choose **Create new branch**.
3. **Write and try the example.** In **Explorer**, open the skill folder. Following its conventions for examples, add the sample lesson and prompt. Try the prompt with the skill in your own AI environment, include the resulting review, and link the example from the skill’s README. Use a GitHub Codespace or local clone for any tests that require a terminal.
4. **Commit from the browser.** Open **Source Control**, review each file’s changes, and select **+** beside the files you want to stage. Enter a message such as `Add worked example for curriculum review` and select **Commit & Push**.
5. **Open a pull request in the editor.** Select the pull request icon at the top of **Source Control**. Choose the original Guild repository and its target branch as the destination. Choose your fork and `add-curriculum-review-example` as the source. Link the enhancement issue, describe how you tried the example, and select **Create**.

### Follow your pull request through review

Watch the pull request for comments and check results. The Guild’s AI steward may help review the contribution. If a reviewer asks for revisions, edit the files on the same branch. With a local clone, commit and run `git push`. In the browser, select **Commit & Push**. The existing pull request updates automatically.

Once the contribution is accepted and any required checks and approvals are complete, a maintainer can merge it. GitHub marks the pull request **Merged**. Guild leaders approve releases, so the change may appear in a later release.

[GitHub’s contribution walkthrough](https://docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-project) · [Using VS Code for the Web](https://docs.github.com/en/codespaces/the-githubdev-web-based-editor)


