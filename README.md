# gaudi-bash themes

This repo holds the prompt themes of [gaudi-bash](https://github.com/g-udi/gaudi-bash). It contains no theme itself: each theme is a repository of its own, included here as a git submodule, and this repo is in turn the `themes` submodule of [gaudi-bash-components](https://github.com/g-udi/gaudi-bash-components).

## Themes

- [**gaudi**](https://github.com/g-udi/gaudi-theme) (folder `gaudi`): a modular prompt made of segments (working directory, git status, language versions, cloud profile, ...), with the slow ones rendered in the background. Its settings are described in [its README](https://github.com/g-udi/gaudi-theme#readme).

## Getting the themes

gaudi-bash fetches them when it is installed. In a clone of this repo:

```bash
git submodule update --init
```

## Adding a theme

A theme is a folder named after the theme with a `<name>.theme.bash` file in it, which gaudi-bash sources. Add its repository as a submodule:

```bash
git submodule add https://github.com/<owner>/<repository> <name>
```

and list it above.
