# Claude Code Workshop Instructions

For pre-requisites, see [docs/PREREQS.md](docs/PREREQS.md).

> **Note:** This contains a lot of pre-approved commands, which in general is a bad idea. Review carefully: [.claude/settings.local.json](.claude/settings.local.json)

Clone this repository, and remove its `.git` folder:

```
git clone git@github.com:xpqz/claudews.git
cd claudews
rm -rf .git
```

Open the cloned repository in VS Code, select a file, and start the Claude Code extension by clicking the little brown "splash" in the tab bar.

Execute the following commands:

```
/rules
/make_project link_check
```
