## git log

Help!
```sh
git help log
```

Shows the list of commits (the most recent commits show up first)
```sh
git log
```

Shows the list of commits and the abbreviated stats
```sh
git log --stat
```

Shows the list of commits and the diff
```sh
git log -p
```

Same as above but limits the output to -n entries (2 in this example)
```sh
git log -p -2
```

Shows the list of commits on a single line
```sh
git log --pretty=oneline
```

Shows the list of formatted commits
```sh
git log --pretty=format:"%h - %an, %ar : %s"
```

Shows the list of formatted commits and a graph
```sh
git log --pretty=format:"%h %s" --graph
```

Shows all commits where commit message contains a given word
```sh
git log -p --grep=word_to_find
```
