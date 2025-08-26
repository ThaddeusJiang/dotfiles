# Cursor Editor dotfiles

```bash
name=$(whoami)
npx degit ThaddeusJiang/dotfiles/.cursor/commands/TJ .cursor/commands/${name:u}
```

## TJ's workflow

- /Plan
- /Coding MVP
- /Coding
- /Review
- /Commit
- /Add memory to Nowledge

## Ignore personal commands

```bash
name=$(whoami)
echo ".cursor/commands/${name:u}" >> ~/.gitignore_global
git config --global core.excludesfile ~/.gitignore_global
```
