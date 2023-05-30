# gitmojima 😊

**gitmojima** is a [gitmoji](https://gitmoji.dev/)-like set, aimed at minimalism and productivity.

> **When Less is More: minimalism and beyond**
>
> The essence of Japanese aesthetic is a concept called **Ma** 間 — the pure, and indeed essential,
void between all things. A total lack of clutter, *Ma* is like a holder within which things can
exist, stand out and have meaning.

## Purpose

[gitmoji](https://gitmoji.dev/) is a loosely visual implementation of [Conventional Commits](https://www.conventionalcommits.org/),
a specification for adding human and machine readable meaning to commit messages.

The current set of gitmoji however stands at 73 items already, with more being added over time.
This high number of available emojis allows for finer granularity, but it is intimidating to make
efficient use of and also causes cognitive hindrance that makes commit history harder to navigate.

**gitmojima** is an attempt to select only a very minimal number of emojis while still
covering most use cases for enhanced productivity.


## Reference

| Emoji | Shortcode                  | Description |
|-------|----------------------------|------------|
| ⚡️ | `:zap:`                       | Improve code |
| 🐛 | `:bug:`                       | Fix a bug |
| ✨ | `:sparkles:`                  | Introduce new features |
| 📝 | `:memo:`                      | Add or update documentation or license |
| 🔧 | `:wrench:`                    | Add or update configuration or development files |
| 🧱 | `:bricks:`                    | Add or update infrastructure build system |
| 🧪 | `:test_tube:`                 | Add or update tests |
| ♻️ | `:recycle:`                   | Refactor code |
| 📦️ | `:package:`                   | Manage dependencies |
| 🔖 | `:bookmark:`                  | Tag or deploy code |
| ⏪️ | `:rewind:`                    | Revert changes |
| 🔀 | `:twisted_rightwards_arrows:` | Merge branches |

## Example of usage

To benefit from an explicit commit history, make use of the [Conventional Commits specification](https://www.conventionalcommits.org/en/v1.0.0/#summary)
structure.

The commit message should be structured as follows:

```
<emoji> [scope?][:?] <description>

[body?]

[footer(s)?]
```

- `emoji`: An emoji from the list.
- `scope`: An optional string that adds contextual information for the scope of the change.
- `description`: A brief explanation of the change.
- `body`: An optional longer explanation of the change.
- `footer(s)`: optional strings that reflect an important information.

## Gitmoji comparison

* only 12 emojis vs 73+
* concise shortcodes for ease of use
* 10 main categories for development
    * ⚡️ for any kind of enhancement (covers ⚡️,💄,📈,🌐,✏️,👽️,🍱,♿️,💡,💬,🗃️,🔊,🔇,🚸,📱,🥚,🔍️,🌱,🚩,💫,🛂,👔,🩺,🧑‍💻,🧵,🦺)
    * 🐛 for all fixes (covers 🐛,🚑️,🔒️,🥅,🩹)
    * ✨ for new features (covers ✨,🎉,💩,💥)
    * 📝 for documentation and license (covers 📝,📄,💸)
    * 🔧 for configuration and development files (covers 🔧,🔨,🙈)
    * 🧱 for infrastructure (covers 👷,💚,🧱)
    * 🧪 for tests (covers ✅,🧪,🤡)
    * ♻️ for refactoring (covers 🎨,🔥,🚨,♻️,🚚,🏗️,🗑️,⚰️)
    * 📦️ for dependency management (covers ➕,➖,⬇️,⬆️,📌)
    * 🔖 for version tags and deployment (covers 🚀,🔖)
* 2 categories for git operations
    * ⏪️ and 🔀 (unchanged)
* not covered because they:
    * are only aimed at features or exploratory branches (🚧,⚗️,🧐)
    * are not part of a typical or sane git workflow (🔐,🍻,📦️,📸)
    * are not self explanatory in how they should be actually used (👥,🏷️)

## References

* [Conventional Commits](https://www.conventionalcommits.org/)
* [How to Write a Git Commit Message](https://cbea.ms/git-commit/)
