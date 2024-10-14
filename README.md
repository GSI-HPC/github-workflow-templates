<!--
SPDX-License-Identifier: CC-BY-SA-4.0
SPDX-FileCopyrightText: 2024 GSI Helmholtzzentrum fuer Schwerionenforschung GmbH <https://gsi.de>
-->

[![REUSE status](https://github.com/GSI-HPC/github-workflow-templates/actions/workflows/reuse.yml/badge.svg)](https://github.com/GSI-HPC/github-workflow-templates/actions/workflows/reuse.yml)
[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8B%20%20%E2%97%8B%20%20%E2%97%8B%20%20%E2%97%8B-red)](https://fair-software.eu)

## How to use in your project

```sh
cd <your repo root>
wget https://github.com/GSI-HPC/github-workflow-templates/raw/refs/heads/main/.pre-commit-config.yaml
mkdir -p .github/workflows
cd .github/workflows
wget https://github.com/GSI-HPC/github-workflow-templates/raw/refs/heads/main/.github/workflows/fair-software.yml
wget https://github.com/GSI-HPC/github-workflow-templates/raw/refs/heads/main/.github/workflows/reuse.yml
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
