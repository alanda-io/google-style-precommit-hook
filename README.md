A handy [pre-commit](http://pre-commit.com/) hook which will run Google's java
code style formatter for you on your code!

Usage:

```
repos:
- repo: https://github.com/alanda-io/google-style-precommit-hook.git
  sha: <commit id>
  hooks:
  - id: google-style-java
```

*Note*: this file stores Google's code style formatter jar in a `.cache/`
directory so that it doesn't need to be re-downloaded each time.  You will
probably want to add `.cache/` to the `.gitignore` file of the project which
uses this hook.

Forked from https://github.com/maltzj/google-style-precommit-hook
