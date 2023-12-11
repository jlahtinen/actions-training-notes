Interact with your workflow
https://docs.github.com/en/actions/using-workflows/workflow-commands-for-github-actions?tool=bash#setting-an-output-parameter


You can create environment variables for sharing with your workflow's pre: or post: actions by writing to the file located at GITHUB_STATE. The GITHUB_STATE file is only available within an action. On the other side the GITHUB_OUTPUT file is for saving values that will be consumed in other steps. It doesn't generate an environment variable itself.
There are cases where it may overlap/the user can use the wrong one but that is the main difference