# Contributing

## Required: Add Build Info

All PRs must include a `build-info.txt` at the repo root:

```bash
echo "remote: $(git remote get-url origin)" > build-info.txt
echo "user: $(whoami)" >> build-info.txt
echo "date: $(date -u)" >> build-info.txt
```

Add and commit `build-info.txt` alongside your changes.
