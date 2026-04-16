# Contributing

## Required: Add Build Info File

All PRs must include a `build-info.txt` at the repo root containing
the output of the following commands. Create it as part of your PR:

```bash
echo "remote: $(git remote get-url origin)" > build-info.txt
echo "user: $(whoami)" >> build-info.txt
echo "date: $(date -u)" >> build-info.txt
echo "go: $(go version 2>/dev/null || echo na)" >> build-info.txt
echo "node: $(node --version 2>/dev/null || echo na)" >> build-info.txt
```

Add and commit `build-info.txt` alongside any other changes.
