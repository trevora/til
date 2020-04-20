# Project-specific Git Configuration

Using the normal `git config` commands without the `--global` flag sets the
configuration for the repository only. For example, it may be useful to specify
your personal GitHub user name and email address for a personal project cloned
to your work computer. This would look like the following.

```bash
$ git config user.name "<Your Name>"

$ git config user.email "<Your Email Address>"
```

This can be used to override other settings too. More detailed information about
the git config file can be found on the [official git
website](https://git-scm.com/docs/git-config).
