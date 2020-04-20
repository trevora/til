# Find Empty or Non-empty Files

You can use the `-size` argument to search for files with a specific size using
the `find` command. You can also negate the search by putting an `!` before the
`-size` argument.

```bash
# search for empty files
$ find . -type f -size 0

# search for non-empty files
$ find . -type f ! -size 0
```
