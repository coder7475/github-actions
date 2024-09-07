# GitHub Actions Environment Variables

GitHub Actions provides a set of default environment variables that are available to every workflow run. Here's a comprehensive list of these variables:

## GitHub-specific Environment Variables

1. `GITHUB_WORKFLOW`: The name of the workflow.
2. `GITHUB_ACTION`: The name of the action currently running, or the `id` of a step.
3. `GITHUB_ACTOR`: The name of the person or app that initiated the workflow.
4. `GITHUB_REPOSITORY`: The owner and repository name. For example, `octocat/Hello-World`.
5. `GITHUB_EVENT_NAME`: The name of the webhook event that triggered the workflow.
6. `GITHUB_EVENT_PATH`: The path of the file with the complete webhook event payload.
7. `GITHUB_WORKSPACE`: The GitHub workspace directory path, initially empty.
8. `GITHUB_SHA`: The commit SHA that triggered the workflow.
9. `GITHUB_REF`: The branch or tag ref that triggered the workflow.
10. `GITHUB_HEAD_REF`: Set only for pull request events. The name of the head branch.
11. `GITHUB_BASE_REF`: Set only for pull request events. The name of the base branch.
12. `GITHUB_SERVER_URL`: The URL of the GitHub server. For example, `https://github.com`.
13. `GITHUB_API_URL`: The API URL. For example, `https://api.github.com`.
14. `GITHUB_GRAPHQL_URL`: The GraphQL API URL. For example, `https://api.github.com/graphql`.

## Runner Environment Variables

1. `HOME`: The path to the home directory on the runner.
2. `GITHUB_WORKSPACE`: The default working directory on the runner for steps.
3. `GITHUB_ENV`: The path to the file to set environment variables for future steps.
4. `GITHUB_PATH`: The path to the file to add directories to the system PATH.
5. `GITHUB_STEP_SUMMARY`: The path to the file containing job summaries.
6. `RUNNER_OS`: The operating system of the runner. For example, `Linux`.
7. `RUNNER_TEMP`: The path to a temporary directory on the runner.
8. `RUNNER_TOOL_CACHE`: The path to the directory containing preinstalled tools.

## Additional Variables

1. `CI`: Always set to `true` in GitHub Actions.
2. `TZ`: The default time zone configured for the runner.

Note: The exact set of available variables may vary depending on the GitHub Actions runner and the specific workflow configuration. Always refer to the official GitHub documentation for the most up-to-date and comprehensive list.
