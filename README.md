
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
| p    | `pnpm`  |  Fast, disk space efficient package manager |
| pi    | `pnpm init`  |  pnpm init |
| pin   | `pnpm install`  |  Is used to install all dependencies for a project. |
| pa    | `pnpm add`  |  Installs a package and any packages that it depends on. |
| pad   | `pnpm add -D`  |  Install the specified packages as devDependencies. |
| pao   | `pnpm add -O`  |  Install the specified packages as optionalDependencies. |
| pae   | `pnpm add -E`  |  Saved dependencies will be configured with an exact version rather than using pnpm's default semver range operator. |
| pap   | `pnpm add --save-peer`  |  Using --save-peer will add one or more packages to peerDependencies and install them as dev dependencies. |
| pag   | `pnpm add --global`  |  Install a package globally. |
| paw   | `pnpm add --workspace`  |  Only adds the new dependency if it is found in the workspace. |
| pup   | `pnpm up`  |  Updates packages to their latest version based on the specified range. |
| pupg   | `pnpm up --global`  |  Update global packages. |
| pupw   | `pnpm up --workspace`  |  Tries to link all packages from the workspace. |
| pupl   | `pnpm up -L`  |  Ignores the version range specified in package.json. Instead, the version specified by the latest tag will be used. |
| prm   | `pnpm remove`  |  Removes packages from node_modules and from the project's package.json. |
| prmg   | `pnpm remove --global`  |  Remove a global package. |
| prmr   | `pnpm remove -r`  |  When used inside a workspace, removes a dependency (or dependencies) from every workspace package. |
| prmd   | `pnpm remove -D`  |  Only remove the dependency from devDependencies. |
| prmo   | `pnpm remove -O`  |  Only remove the dependency from optionalDependencies. |
| prmp   | `pnpm remove -P`  |  Only remove the dependency from dependencies. |
| plg   | `pnpm link --global`  |  Links package from location where this command was executed or specified via --dir option to global node_modules, so it can be referred from another package with pnpm link --global <pkg>. |
| pul   | `pnpm unlink`  |  Unlinks a system-wide package (inverse of pnpm link). |
| pim   | `pnpm import`  |  generates a pnpm-lock.yaml from another package manager's lockfile. Supported source files:`package-lock.json`,`npm-shrinkwrap.json`,`yarn.lock` |
| prb   | `pnpm rebuild`  |  Rebuild a package. |
| ppr   | `pnpm prune`  |  Removes unnecessary packages. |
| pf   | `pnpm fetch`  |  Fetch packages from a lockfile into virtual store, package manifest is ignored. |
| pau   | `pnpm audit`  |  Checks for known security issues with the installed packages. |
| pls   | `pnpm list`  |  This command will output all the versions of packages that are installed, as well as their dependencies, in a tree-structure. |
| pout   | `pnpm outdated`  |  Checks for outdated packages. The check can be limited to a subset of the installed packages by providing arguments (patterns are supported). |
| poutg   | `pnpm outdated --global`  |  List outdated global packages. |
| pwhy   | `pnpm why`  |  Shows all packages that depend on the specified package. |
| pwhyg   | `pnpm why --global`  |  List packages in the global install directory instead of in the current project. |
| prun   | `pnpm run`  |  Runs a script defined in the package's manifest file. |
| pt   | `pnpm test`  |  Runs an arbitrary command specified in the package's test property of its scripts object. |
| pe   | `pnpm exec`  |  Execute a shell command in scope of a project. |
| px   | `pnpm dlx`  |  Fetches a package from the registry without installing it as a dependency, hotloads it, and runs whatever default command binary it exposes. |
| pc   | `pnpm create`  |  Create a project from a create-* starter kit. |
| pst   | `pnpm start`  |  Runs an arbitrary command specified in the package's start property of its scripts object. If no start property is specified on the scripts object, it will attempt to run node server.js as a default, failing if neither are present. |
| pd   | `pnpm dev`  |  Run pnpm dev command. |
| pb   | `pnpm build`  |  Run pnpm build command. |
| penv   | `pnpm env`  |  Manages the Node.js environment. |
| ppub   | `pnpm publish`  |  Publishes a package to the registry. |
| ppubt   | `pnpm publish --tag`  |  Publishes the package with the given tag. By default, pnpm publish updates the latest tag. |
| ppubf   | `pnpm publish --force`  |  Try to publish packages even if their current version is already found in the registry. |
| pp   | `pnpm pack`  |  Create a tarball from a package. |
| prec   | `pnpm recursive`  |  Runs a pnpm command recursively on all subdirectories in the package or every available workspace. |
| ps   | `pnpm store`  |  Managing the package store. |
| psv   | `pnpm server`  |  Manage a store server. |
| pr   | `pnpm root`  |  Prints the effective modules directory. |
| prg   | `pnpm root -g`  |  The global package's modules directory is printed. |
| pbin   | `pnpm bin`  |  Prints the directory into which the executables of dependencies are linked. |
| pbing   | `pnpm bin -g`  |  Prints the location of the globally installed executables. |
| pv   | `pnpm version`  |  pnpm version info. |
| ph   | `pnpm help`  |  pnpm help info. |