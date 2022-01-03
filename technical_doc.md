<!---Jaepeto-section-fixed: top1-start--->
> A Discord Rich Presence Client in Python? Looks like you've come to the right place.

[![GitHub stars](https://img.shields.io/github/stars/qwertyquerty/pypresence.svg?style=for-the-badge&label=Stars)](https://github.com/qwertyquerty/pypresence) [![license](https://img.shields.io/github/license/qwertyquerty/pypresence.svg?style=for-the-badge)](https://github.com/qwertyquerty/pypresence/blob/master/LICENSE) ![GitHub last commit](https://img.shields.io/github/last-commit/qwertyquerty/pypresence.svg?style=for-the-badge) ![GitHub top language](https://img.shields.io/github/languages/top/qwertyquerty/pypresence.svg?style=for-the-badge) ![PyPI](https://img.shields.io/pypi/v/pypresence.svg?style=for-the-badge)

## NOTE: Only Python versions 3.8 and above are supported.

### [Documentation](https://qwertyquerty.github.io/pypresence/html/index.html), [Discord Server](https://discord.gg/JF3kg77), [Patreon](https://www.patreon.com/qwertyquerty)

----------

**Use this badge in your project's Readme to show you're using pypresence! The markdown code is below.**

[![pypresence](https://img.shields.io/badge/using-pypresence-00bb88.svg?style=for-the-badge&logo=discord&logoWidth=20)](https://github.com/qwertyquerty/pypresence)

```markdown
[![pypresence](https://img.shields.io/badge/using-pypresence-00bb88.svg?style=for-the-badge&logo=discord&logoWidth=20)](https://github.com/qwertyquerty/pypresence)
```
<!---Jaepeto-section-fixed: top1-end--->

<!---Jaepeto-section-group: helloworld-start--->
## Getting started

<!---Jaepeto-section-helloworld: setup-start--->

### Requirements

* python 3.6 or greater

<details>
  <summary>Click to see why</summary>

  The code uses f-strings in `pypresence/utils.py`
</details>



`pypresence` is pip-installable.
Clone the repository
and run `pip install -e .` in top-level directory
to install package in locally.
Alternatively,
install from pypi


<!---Jaepeto-section-helloworld: setup-end--->

<!---Jaepeto-section-helloworld: entrypoints-start--->


## Entrypoints

There are 5 source code objects in top-level `__main__`/`__init__`:

### pypresence.baseclient.BaseClient

```python
class BaseClient(self, client_id: str, **kwargs)
        Possible kwargs include "pipe", "loop", "handler", "isasync"
        Can raise `PyPresenceError`, `InvalidArgument`
```

`BaseClient` is a base class;
it has child classes:

* `pypresence/client/Client`
* `pypresence/client/AioClient`
* `pypresence/presence/Presence`
* `pypresence/presence/AioPResence`

`BaseClient` has asynchronous methods.

### pypresence.client.Client

```python
class Client(self, *args, **kwargs)
```

`Client` inherits from `pypresence/baseclient/BaseClient`

### pypresence.client.AioClient

```python
class AioClient(self, *args, **kwargs)
```

`AioClient` inherits from `pypresence/baseclient/BaseClient`


### pypresence.presence.Presence

```python
class Presence(self, *args, **kwargs)
```

`Presence` inherits from `pypresence/baseclient/BaseClient`

### pypresence.presence.AioPresence

```python
class AioPresence(self, *args, **kwargs)
```

`AioPresence` inherits from `pypresence/baseclient/BaseClient`


<!---Jaepeto-section-helloworld: entrypoints-end--->

## Concepts



<!---Jaepeto-section-group: helloworld-end--->

<!--Jaepeto-section-group: developers-start--->

## Developers

<!---Jaepeto-section-developers: ci-start--->
The project uses GitHub Actions for CI/CD.

| File | Purpose |
|:-----|:--------|
| .github/workflows/lint_python | Runs on pull request or push on every branch. Runs code linting (black, isort, mypy, bandit) and testing (pytest) |
| .github/workflows/publish-to-pypi | Runs on release. Uploads package to pypi |


<!---Jaepeto-section-developers: ci-end--->

There are no unit tests for `pypresence`.

### Entrypoints

These entrypoints are broken down into the following modules:

* `pypresence.client` has 2 entrypoints
* `pypresence.presence` has 2 entrypoints
* `pypresence.baseclient` has 1 entrypoints

<!---Jaepeto-section-group: developers-end--->

<!---Jaepeto-section-fixed: bottom2-start--->
----------

## Examples

Examples can be found in the [examples](https://github.com/qwertyquerty/pypresence/tree/master/examples) directory, and you can contribute your own examples if you wish, just read [examples.md](https://github.com/qwertyquerty/pypresence/blob/master/examples/examples.md)!

<!---Jaepeto-section-fixed: bottom2-end--->
<!---Jaepeto-section-fixed: bottom1-start--->
## Documentation

> **NOTE**: You need an **authorized app** to do anything besides rich presence!

####  [pypresence Documentation](https://qwertyquerty.github.io/pypresence/html/index.html)
####  [Discord Rich Presence Documentation](https://discordapp.com/developers/docs/rich-presence/how-to)
####  [Discord RPC Documentation](https://discordapp.com/developers/docs/topics/rpc)
####  [pyresence Discord Support Server](https://discord.gg/JF3kg77)
####  [Discord API Support Server](https://discord.gg/discord-api)



----------
Written by: [qwertyquerty](https://github.com/qwertyquerty)

Notable Contributors: [GiovanniMCMXCIX](https://github.com/GiovanniMCMXCIX), [GhostofGoes](https://github.com/GhostofGoes)
<!---Jaepeto-section-fixed: bottom1-end--->