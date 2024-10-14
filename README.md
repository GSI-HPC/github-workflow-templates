<!--
SPDX-License-Identifier: CC-BY-SA-4.0
SPDX-FileCopyrightText: 2024 GSI Helmholtzzentrum fuer Schwerionenforschung GmbH <https://gsi.de>
-->

## How to use in your project

```sh
cd <your repo root>
wget https://github.com/GSI-HPC/github-workflow-templates/raw/refs/heads/master/.pre-commit-config.yaml
mkdir -p .github/workflows
cd .github/workflows
wget https://github.com/GSI-HPC/github-workflow-templates/raw/refs/heads/master/fair-software.yml
wget https://github.com/GSI-HPC/github-workflow-templates/raw/refs/heads/master/reuse.yml
cd ../..
git add .pre-commit-config.yaml .github/workflows/fair-software.yml .github/workflows/reuse.yml
```

To enable the REUSE pre-commit hook install `pre-commit` and then install the 
configured pre-commit hook:

```sh
pip install pre-commit
pre-commit install
```

## Badges

The fair-software workflow will produce the Markdown to paste into your 
README.md

For a REUSE badge, it is recommended to simply add (you can generate this badge 
on the GitHub workflow webpage):

```markdown
[![REUSE status](https://github.com/GSI-HPC/<repo name>/actions/workflows/reuse.yml/badge.svg)](https://github.com/GSI-HPC/<repo name>/actions/workflows/reuse.yml)
```
