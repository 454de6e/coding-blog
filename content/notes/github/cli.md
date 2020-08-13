# GitHub CLI

https://cli.github.com/manual/

## Authentication

Recently GitHub CLI started honoring `GITHUB_TOKEN` which is sourced via
`~/.env` in my `~/.zshrc`. This token requires the following permissions:

- `public_repo`
- `read:org`
- `read:discussion`

## Useful commands

### Clone a repo

```
gh repo clone <user/org>/<repo>
```

You need to set your protocol preference in `~/.config/gh/config.yml` by setting
key `git_protocol` to `https` or `ssh`.

### Pull requests

```
gh pr list
```

```
gh pr view <number> -w
```