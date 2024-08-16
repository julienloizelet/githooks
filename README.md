# Git hooks

---
> Some reusable git hooks
---


## Usage

### Per repository usage

- Clone this repository
- copy a hook in the `.git/hooks` folder of your project
- make it executable if necessary: `chmod +x .git/hooks/<hook-name>`

### Global usage

See https://stackoverflow.com/a/37293198/7497291

**!!Warning!!** setting global hooks path disables all local hooks in your repos

- Clone this repository in some `/path/to/the/clone/` folder.
- make it executable if necessary: `chmod +x /path/to/the/clone/hooks/<hook-name>`
- `git config --global core.hooksPath /path/to/the/clone/hooks`

## Hooks

### commit-msg

Check if the commit message follows a custom format.

This format is slightly different from the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) format:

- The type is mandatory and must be one of the following:
  - `feat`: a new feature
  - `fix`: a bug fix
  - `docs`: documentation only changes
  - `style`: changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
  - `refactor`: a code change that neither fixes a bug nor adds a feature
  - `ci`: changes to CI configuration files and scripts
  - `test`: adding missing tests or correcting existing tests
  - `chore`: changes to the build process or auxiliary tools and libraries such as documentation generation
  - `comment`: changes that only affect comments

- The scope is mandatory (wildcard `*` is allowed)

- Last sentence must start with uppercased letter

- An optional prefix is allowed and must be one of the following:
  - `(#XXXX)`: where `XXXX` is an integer (related to an issue for example)


## License

[MIT](LICENSE)

## Contribute

Anyone is welcome to submit a pull request to this repository.


**Contributed and maintained by [julienloizelet](https://github.com/julienloizelet)**
