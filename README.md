# gitmojima 😊

**gitmojima** is an emoji guide for commit messages, aimed at minimalism and productivity.

> **When Less is More: minimalism and beyond**
>
> The essence of Japanese aesthetic is a concept called **Ma** 間 — the pure, and indeed essential,
void between all things. A total lack of clutter, *Ma* is like a holder within which things can
exist, stand out and have meaning.

## Purpose

[gitmoji](https://gitmoji.dev/) aims to enhance commit message readability by using emojis. However, the current set of 73 items is overwhelming, making it difficult to select the right emoji and understand their intended meanings, which ironically complicates commit history navigation.

**gitmojima** is a formal specification that refines emoji usage in commit messages through a more focused set, balancing simplicity and coverage. This allows developers to focus on the actual content of their commits.

It aligns with the [Conventional Commits](https://www.conventionalcommits.org/) specification.

## Reference

| Emoji       | Shortcode                  | Conventional type | Description            |
|-------------|----------------------------|-------------------|------------------------|
| :sparkles:  | `:sparkles:`               | feat              | Introduce new features |
| :bug:       | `:bug:`                    | fix               | Fix a bug |
| :zap:       | `:zap:`                    | perf              | Improve code |
| :memo:      | `:memo:`                   | docs              | Add or update documentation or license |
| :wrench:    | `:wrench:`                 | build             | Add or update configuration or development files |
| :bricks:    | `:bricks:`                 | ci                | Add or update infrastructure build system |
| :art:       | `:art:`                    | style             | Add or update UI or style files |
| :test_tube: | `:test_tube:`              | test              | Add or update tests |
| :recycle:   | `:recycle:`                | refactor          | Refactor code |
| :package:   | `:package:`                | chore             | Manage dependencies |
| :bookmark:  | `:bookmark:`               | chore             | Tag or deploy code |
| :rewind:    | `:rewind:`                 | revert            | Revert changes |

## Specification

To benefit from an explicit commit history, make use of the [Conventional Commits specification](https://www.conventionalcommits.org/en/v1.0.0/#summary)
structure.

The commit message should be structured as follows:

```
<emoji> [scope?][:?] <description>

[body?]

[footer(s)?]
```

- `emoji`: An emoji shortcode from the list
    * Use *text shortcode* rather than unicode notation
- `scope`: An optional string that adds contextual information for the scope of the change
- `description`: A brief explanation of the change
    * Limit the subject line to 50 characters (not including the shortcode length)
    * Capitalize the subject line
    * Do not end the subject line with a period
    * Use the imperative mood in the subject line
- `body`: An optional longer explanation of the change
    * Separate subject from body with a blank line
    * Wrap the body at 72 characters
    * Use the body to explain *what* and *why* vs. *how*
- `footer(s)`: optional strings that reflect an important information


## Usage

```
:shortcode: Summarize changes in around 50 characters or less

More detailed explanatory text, if necessary. Wrap it to about 72
characters or so. In some contexts, the first line is treated as the
subject of the commit and the rest of the text as the body. The
blank line separating the summary from the body is critical (unless
you omit the body entirely); various tools like `log`, `shortlog`
and `rebase` can get confused if you run the two together.

Explain the problem that this commit is solving. Focus on why you
are making this change as opposed to how (the code explains that).
Are there side effects or other unintuitive consequences of this
change? Here's the place to explain them.

Further paragraphs come after blank lines.

- Bullet points are okay, too

- Typically a hyphen or asterisk is used for the bullet, preceded
by a single space, with blank lines in between, but conventions
vary here

If you use an issue tracker, put references to them at the bottom,
like this:

Resolves: #123
See also: #456, #789
```

## Dependabot

If using [dependabot](https://docs.github.com/en/code-security/dependabot), you can
[customize dependency updates](https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/customizing-dependency-updates)
to correspond to the above specification.

In `.github/dependabot.yml`, use make use of the `commit-message` option. For example:

```
version: 2
updates:
- package-ecosystem: "gradle"
directory: "/"
schedule:
interval: "weekly"
commit-message:
# Prefix all commit messages with emoji
prefix: ":package: "
include: "scope"
```

See [Configuration options](https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file)
for all available options.

## References

* [Conventional Commits](https://www.conventionalcommits.org/)
* [How to Write a Git Commit Message](https://cbea.ms/git-commit/)
