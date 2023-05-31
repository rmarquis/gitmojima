# gitmojima 😊

**gitmojima** is a [gitmoji](https://gitmoji.dev/)-like set, aimed at minimalism and productivity.

> **When Less is More: minimalism and beyond**
>
> The essence of Japanese aesthetic is a concept called **Ma** 間 — the pure, and indeed essential,
void between all things. A total lack of clutter, *Ma* is like a holder within which things can
exist, stand out and have meaning.

## Purpose

[gitmoji](https://gitmoji.dev/) enhances commit message readability by using emojis. However, the
current gitmoji set consists of an extensive collection of 73 items, leading to several challenges:

* It is overwhelming and causes cognitive hindrance when efficiently using them.
* Navigating the commit history becomes challenging due to the sheer volume of emojis.
* Its abundance of emojis often leads to confusion and difficulty in understanding their intended meaning.
* The lack of clarity in provided emoji usage explanations hinders standardization.

**gitmojima** is a formal specification that improves the use of emojis in commit messages through
a more focused and standardized set. It streamlines the process, enhances productivity, and allows
developers to focus on the content of their commits.

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

By achieving a balance between simplicity and coverage, gitmojima provides:

* **Streamlined Selection**: to simplify decision-making for developers.
* **Enhanced Comprehension**: to reduce confusion and improve understanding.
* **Improved Standardization**: to promote consistency with a formal specification.
* **Increased Efficiency**: to save time, improve communication and enhance productivity.

In details:

* only 12 emojis vs 73+
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
* some categories are not covered, because they:
    * are only aimed at features or exploratory branches (🚧,⚗️,🧐)
    * are not part of a typical or sane git workflow (🔐,🍻,📦️,📸)
    * are not self explanatory in how they should be actually used (👥,🏷️)
* concise shortcodes for main categories
* easy to use and easy to remember

## References

* [Conventional Commits](https://www.conventionalcommits.org/)
* [How to Write a Git Commit Message](https://cbea.ms/git-commit/)
