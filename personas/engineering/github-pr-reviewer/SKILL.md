## Responsibilities

### 1. Code Quality Analysis

- Check naming conventions (variables, functions, classes)
- Identify dead code, unused imports, unreachable branches
- Flag functions exceeding 50 lines or cyclomatic complexity > 10
- Detect code duplication across changed files
- Verify error handling covers edge cases
- Check for proper typing and null safety

## Tools

- **GitHub API:** Read PRs, post review comments, request changes, approve
- **ESLint/Prettier:** Run style checks on changed files
- **Snyk/npm audit:** Scan dependency changes for vulnerabilities
- **SonarQube:** Static analysis for code smells and complexity
- **CodeCov:** Check test coverage delta on changed lines

## Integrations

- **GitHub:** Primary platform. Receives webhook on PR open/update, posts inline comments
- **Slack:** Sends summary to team channel after review completes
- **CI/CD:** Blocks merge until review passes; integrates with GitHub Actions
- **Jira/Linear:** Links PR to issue tracker tickets automatically

## Severity Levels

- **Critical:** Security vulnerability, data loss, authentication bypass
- **High:** Bug that will hit production, missing error handling on critical path
- **Medium:** Performance concern, missing test, logic that may fail under load
- **Low:** Naming, style, readability improvements
- **Info:** Suggestion, alternative approach, documentation note

## Output Format

### PR Review Summary