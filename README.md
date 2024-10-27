# netquality

![speedtest logo](https://m.media-amazon.com/images/I/516GU1+37yL.png)

<p align="center">
    <a href="https://github.com/YisusChrist/netquality/issues">
        <img src="https://img.shields.io/github/issues/YisusChrist/netquality?color=171b20&label=Issues%20%20&logo=gnubash&labelColor=e05f65&logoColor=ffffff">&nbsp;&nbsp;&nbsp;
    </a>
    <a href="https://github.com/YisusChrist/netquality/forks">
        <img src="https://img.shields.io/github/forks/YisusChrist/netquality?color=171b20&label=Forks%20%20&logo=git&labelColor=f1cf8a&logoColor=ffffff">&nbsp;&nbsp;&nbsp;
    </a>
    <a href="https://github.com/YisusChrist/netquality/stargazers">
        <img src="https://img.shields.io/github/stars/YisusChrist/netquality?color=171b20&label=Stargazers&logo=octicon-star&labelColor=70a5eb">&nbsp;&nbsp;&nbsp;
    </a>
    <a href="https://github.com/YisusChrist/netquality/actions">
        <img alt="Tests Passing" src="https://github.com/YisusChrist/netquality/actions/workflows/github-code-scanning/codeql/badge.svg">&nbsp;&nbsp;&nbsp;
    </a>
    <a href="https://github.com/YisusChrist/netquality/pulls">
        <img alt="GitHub pull requests" src="https://img.shields.io/github/issues-pr/YisusChrist/netquality?color=0088ff">&nbsp;&nbsp;&nbsp;
    </a>
    <a href="https://opensource.org/license/gpl-2-0/">
        <img alt="License" src="https://img.shields.io/github/license/YisusChrist/netquality?color=0088ff">
    </a>
</p>

<p align="center">
    <a href="https://github.com/YisusChrist/netquality/issues/new?assignees=YisusChrist&labels=bug&projects=&template=bug_report.yml">Report Bug</a>
    ·
    <a href="https://github.com/YisusChrist/netquality/issues/new?assignees=YisusChrist&labels=feature&projects=&template=feature_request.yml">Request Feature</a>
    ·
    <a href="https://github.com/YisusChrist/netquality/issues/new?assignees=YisusChrist&labels=question&projects=&template=question.yml">Ask Question</a>
    ·
    <a href="https://github.com/YisusChrist/netquality/security/policy#reporting-a-vulnerability">Report security bug</a>
</p>

_Benchmark your internet connection._
<br>

| Measure speed, ping, jitter and packet loss. | Get a rating to understand and compare results. |
| :------------------------------------------: | :---------------------------------------------: |
|     ![](https://i.imgur.com/K1hF3o6.png)     |      ![](https://i.imgur.com/diodVSM.png)       |

Table of Contents

- [netquality](#netquality)
  - [Dependencies](#dependencies)
  - [Installation](#installation)
    - [From PyPI](#from-pypi)
    - [From source](#from-source)
    - [Installing to system path (Linux)](#installing-to-system-path-linux)
  - [Usage](#usage)
  - [Uninstalling](#uninstalling)
  - [License](#license)
  - [Credits](#credits)

## Dependencies

- [Python 3.8+](https://www.python.org/downloads)
- [poetry](https://python-poetry.org/docs/#installation)
- [speedtest-cli](https://pypi.org/project/speedtest-cli)
- [pythonping](https://pypi.org/project/pythonping)
- [match-func](https://pypi.org/project/match-func)
- [string-grab](https://pypi.org/project/string-grab)

## Installation

### From PyPI

```sh
pipx install netquality
```

### From source

Open a **Terminal** and run the following commands:

```sh
git clone https://github.com/yisuschrist/netquality
cd netquality
poetry install
poetry run netquality
```

### Installing to system path (Linux)

This option is not recommended, as it may cause conflicts with other packages because of the `netquality` dependencies.

Open a **Terminal** and run the following commands:

```sh
git clone https://github.com/yisuschrist/netquality
cd netquality/netquality
mv __main__.py netquality
sudo chmod +x netquality
sudo cp netquality /usr/bin
```

## Usage

You can run netquality from anywhere with the `netquality` command.

> Note: To run netquality from anywhere, it is required to use root privileges due to the [pythonping](https://pypi.org/project/pythonping) library. See the reason [here](https://github.com/alessandromaggio/pythonping?tab=readme-ov-file#why-do-i-need-to-be-root-to-use-pythonping). Because of this, it is currently being studied to replace it with [pingparsing](https://github.com/thombashi/pingparsing) which may be a simpler approach.

## Uninstalling

To uninstall `netquality`, simply remove the installation folder and the executables from the system path. If you installed it from PyPI, you can use the following commands:

```sh
pipx uninstall netquality
```

## License

`netquality` is released under the [GPL-2.0 License](https://opensource.org/license/gpl-2-0).

## Credits

> [!NOTE]
> Credits to [Julynx](https://github.com/Julynx) for creating the script. I only make improvements in his code based on my preferences to customize it. All the ideas and the base of the script are his.
