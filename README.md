
# Pnpm plugin

This plugin adds completion for the [Pnpm package manager](https://pnpm.io/),
as well as some aliases for common Pnpm commands.

To use it, add `pnpm` to the plugins array in your zshrc file:

```zsh
zinit light zhanghecool/zsh-shortcut-pnpm
```

## Aliases

| Alias | Command | Description |
| ----- | :--- | ---: |
| ipnpm    | `wget -qO- https://get.pnpm.io/install.sh \| sh -`  |  Installation pnpm |
| p    | `pnpm`  |  pnpm |
| pi    | `pnpm init`  |  pnpm init |
| pin   | `pnpm install`  |  `pnpm install` is used to install all dependencies for a project. |
| pa    | `pnpm add`  |  Installs a package and any packages that it depends on. By default, any new package is installed as a production dependency. |