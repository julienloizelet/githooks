# Git hooks

---
> Some reusable git hooks
---


## Usage

## Per repository usage

- Clone this repository
- copy a hook in the `.git/hooks` folder of your project
- make it executable if necessary: `chmod +x .git/hooks/<hook-name>`

## Global usage

**!!Warning!!** setting a global hooks path disables all local hooks in you repos

- Clone this repository in some `/path/to/the/clone/` folder.
- make it executable if necessary: `chmod +x /path/to/the/clone/hooks/<hook-name>`
- `git config --global core.hooksPath /path/to/the/clone/hooks`



## License

[MIT](LICENSE)

## Contribute

Anyone is welcome to submit a pull request to this repository.


**Contributed and maintained by [julienloizelet](https://github.com/julienloizelet)**
