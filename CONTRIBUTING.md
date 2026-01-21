# Contributing to Perplexity Chat Zsh Script

Thank you for your interest in contributing to this project! This document provides guidelines and instructions for proposing changes.

## How to Contribute

Since this project is currently maintained by a single maintainer, contributions are welcome through the following methods:

### Issues (Recommended for Feedback)

Open an **issue** to:
- Report bugs or unexpected behavior
- Suggest new features or improvements
- Ask questions about usage
- Propose localization changes (French/English support)
- Provide general feedback

Issues are the preferred method for community input and require no Git experience.

### Pull Requests (For Code Changes)

For code contributions:

1. **Fork the repository** to create your own copy
2. **Create a feature branch** from `main`:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Make your changes** following the guidelines below
4. **Test your changes** thoroughly before submitting
5. **Push to your fork**:
   ```bash
   git push -u origin feature/your-feature-name
   ```
6. **Submit a pull request** describing:
   - What changes you made and why
   - Any new dependencies or requirements
   - How to test your changes
   - Localization impact (if applicable)

## Code Guidelines

- **Comments**: Currently in French. Localization to English or other languages welcome via PR
- **Commands**: Currently in French. Localization proposals accepted via issues/PRs
- **Commits**: Use English for commit messages (standard GitHub practice)
- **Style**: Follow existing code conventions in the project
- **Testing**: Ensure your changes don't break existing functionality
- **Localization**: When translating, provide both original + new language versions for review

## Review Process

All pull requests will be reviewed by the maintainer for:
- Code quality and consistency
- Functionality and correctness
- Documentation completeness
- Compatibility with the project goals
- Localization quality (if applicable)

The maintainer reserves the right to:
- Request modifications before merging
- Close pull requests that don't align with project scope
- Rebase, squash, or modify commits as needed
- Choose final localization direction

## Branch Protection

The **`main`** branch is protected and represents the stable, published version. Only the maintainer can merge directly to `main`[1][2].

## License

By contributing to this project, you agree that your contributions will be licensed under the same license as the project.

## Questions?

Feel free to open an issue with the `question` label if you have any doubts about the contribution process.

---

**Current Status**: Single maintainer. For significant contributions, localization changes, or feature requests, please open an issue first to discuss your ideas.
