# Jargonary Website ([jargonary.org](https://jargonary.org))
[![CircleCI Build Status](https://circleci.com/gh/jargonary/jargonary.org.svg?style=shield)](https://app.circleci.com/pipelines/github/jargonary/jargonary.org) [![GitHub License](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jargonary/jargonary.org/trunk/LICENSE)

This is the public repository for <https://jargonary.org>, a static website generated by [Hugo](https://GoHugo.io/).


## Run Locally

You can run this website locally by cloning this repo and serving it with Hugo.
If you don't already have Hugo installed, visit Hugo Docs and follow the [Hugo Install Instructions](https://gohugo.io/getting-started/installing/).

```
git clone https://github.com/jargonary/jargonary.org.git
cd jargonary.org
hugo -s src serve
```

You'll then be able to view the site in your browser at `http://localhost:1313/`.


## How to add a term to the website

You can add a new term to a topic on Jargonary by creating a Markdown file in the directory for the topic.
For example, terms for "SaaS" would go in `src/content/saas/new-term.md`.
Hugo has a `new` command allowing you to use a template when creating this file.
To add a term to "SaaS" for example, you would run:

```bash
hugo -s src new saas/new-term.md
```

That will create a template file for you at the correct location.
Then you can edit the file and fill in the appropriate information.

**Note: If the term has an acronym, use that acronym as the filename. If it doesn't, use the full term, all lowercase, with hyphens instead of spaces, as the filename.**


## License

The source code for `jargonary.org` is licensed under the MIT license.
This repo's license can be found [here](./LICENSE).
