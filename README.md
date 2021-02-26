# acend guidelines

## Documentation style guide

Labs and documentation adhere to the [Kubernetes Documentation Style Guide](https://kubernetes.io/docs/contribute/style/style-guide/).


## Git commit messages

Git commit messages follow the seven rules of [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/).


## Markdown formatting

Markdown sources are linted with [David Anson's markdownlint](https://github.com/DavidAnson/markdownlint) tool using [this configuration](acend.json).\
These overrule the recommendations in the [Kubernetes Documentation Style Guide](https://kubernetes.io/docs/contribute/style/style-guide/).


### Titles

Titles should generally be short and meaningful. Use the same case sensitivity as in the paragraphs.

| Do            | Don't                                             |
| ------------- | ------------------------------------------------- |
| Add backend   | Add Backend                                       |
| Add backend   | Add a MariaDB database to the awesome application |


### Tasks

Lab task titles are written in the following form: `Task <lab/section/chapter number>.<task number>: <Task title>`

Use the shortcode `{{< param sectionnumber >}}` as the `<lab/section/chapter number>` part.

Example: `## Task {{< param sectionnumber >}}.1: Install Kustomize`


### Notes and warnings

Notes and warnings are highlighted in a particular way using `alert` shortcodes.

* Notes: `{{% alert title="Note" color="primary" %}}`
* Warning: `{{% alert title="Warning" color="secondary" %}}`


### Specific terms

* "Web console" for everything that refers to a web user interface ("web GUI"/"WebGUI"/"Web UI"/...)
