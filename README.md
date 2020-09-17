# todo-actions-lite

Like [`todo-actions`](https://github.com/dtinth/todo-actions) but more lightweight.

TODO: #1 Write more information about what this project is about

## Differences

| todo-actions | todo-actions-lite |
| ------------ | ----------------- |
| Written in **JavaScript**. | Written in **Ruby**. |
| Creates an issue for you when encountering a TODO comment. | You have to create an issue yourself. You can use GitHub Issues and Pull Requests VSCode extension to make this process easier. |
| Codebase designed to be tested and maintainable. Can be reused in multiple repos. | Codebase designed to be copy-pasted into a repository and customized there. |

## Usage

The intended usage for this action is for you to totally own the code, giving you full control to change the action’s behavior to suit your needs.
No need for a configuration file when you can just edit the code.

Copy the directory `.github/actions/todo` and `.github/workflows/todo.yml` into your repository. You can run this command to do it:

```sh
curl -L https://github.com/dtinth/todo-actions-lite/tarball/main \
  | bsdtar xvzf - --strip-components=1 --include='*/.github/actions/todo' --include='*/.github/workflows/todo.yml'
```

**Note:** The default workflow runs the action on branch `main`. If your default branch is not `main`, make sure to change it accordingly.
