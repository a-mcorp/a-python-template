<sup>This project has been generated using ['A-Python-Template' (APT)](https://github.com/a-mcorp/a-python-template).</sup>

# {project-name}

## Metadata
<!-- - Author: {author-name}/{author-alias}. -->
- Name: '{project-name}'.
- Purpose: {project-summary}.
- Format: {project-format}.
- License:
  - This project's license: [MIT No Attribution](LICENSE) <!-- the template's own licence: in a project created from it, replace `LICENSE`, this line and the licence fields (`pyproject.toml`, AppImage `appdata.xml`) with the project's licence -->
  <!-- - Dependency-1: [{dependency-1-name}]({dependency-1-license}) -->
  <!-- - Dependency-2: [{dependency-2-name}]({dependency-2-license}) -->

## Features
<table>
<tr>
<th colspan="2">Features</th>
</tr>
<tr>
<td colspan="2">

- {feature-1}
- {feature-2}

</td>
</tr>
<tr>
<th>{example-1-title}</th>
<th>{example-2-title}</th>
</tr>
<tr>
<td align="center"><img src="docs/{example-1-image}" alt="{example-1-title}" width="480"></td>
<td align="center"><img src="docs/{example-2-image}" alt="{example-2-title}" width="370"></td>
</tr>
</table>

## Setup
<table>
<tr>
<th>Dependencies</th>
<th>Usage</th>
</tr>
<tr>
<td valign="top">

  - Version: __{python-version}__
  - Manager: [__{python-manager}__]({python-manager-url})
  <!-- [__pip__](https://docs.python.org/3/installing/index.html) -->
  <!-- [__poetry__](https://github.com/python-poetry/poetry) -->
  <!-- [__uv__](https://github.com/astral-sh/uv) -->
  - Toolset:
    - [pyproject.toml](https://packaging.python.org/en/latest/guides/writing-pyproject-toml/)
    - [venv](https://docs.python.org/3/library/venv.html)
    - [pre-commit](https://github.com/pre-commit/pre-commit) (hooks)
      - [ruff](https://github.com/astral-sh/ruff)
      - [mypy](https://github.com/python/mypy)

</td>
<td valign="top">

  - project
    - {...}
  - local tests
    - {...}
    <!-- - `{project-name}/tests.py` -->
  - local CI
    <!-- - `pre-commit run --all-files` -->
    <!-- - - Files must be first added by `git add` for `pre-commit run` to detect. -->
    <!-- - - `pre-commit run` will install a .venv inside `~/.cache/pre-commit/` -->
  - local CD
    - AppImage deployment
      - See [AppImage/README.md](AppImage/README.md)

</td>
</tr>
</table>

### Installation
{...}
<!-- Venv -->
  <!-- - Windows
    - `cd "C:\Users\{user-name}\AppData\Local\Programs\Python\Launcher"`
    - `.\py.exe -{python-version} -m venv "{path}/{project-name}/venv-{python-version}"` <sub>suggested</sub>
    - everything below
  - Linux
    - `python{python-version} -m venv {path}/{project-name}/venv-{python-version}` <sub>suggested</sub>
    - everything below
  1. `cd {path}/{project-name}`
  2. `source venv-{python-version}/bin/activate`
  3. `pip install --upgrade pip`
  4. `pip install .`
  5. double check with `which python` (Linux) -->

### Repository structure
```
.
├── .github
│   ├── CHANGELOG_TEMPLATE         # Template for CHANGELOG.md
│   ├── CODEOWNERS_TEMPLATE        # Template for CODEOWNERS
│   ├── PULL_REQUEST_TEMPLATE      # Additional pull request templates
│   ├── CODEOWNERS                 # Code owners
│   └── pull_request_template.md   # Default pull request template
├── AppImage                       # AppImage recipe and build guide
├── docs                           # Documentation assets
├── {project-name}                 # Project source code
├── .pre-commit-config.yaml        # pre-commit hooks (local CI)
├── CHANGELOG.md                   # Project changelog
├── LICENSE                        # Project license
├── pyproject.toml                 # Project metadata and tool configuration
└── README.md                      # Project documentation
```

<!-- 
## Troubleshooting
-->