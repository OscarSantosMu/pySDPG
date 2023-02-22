# pySDPG

[![emoji-log](https://img.shields.io/badge/%F0%9F%9A%80-emoji%20log-gray.svg?colorA=3F3750&colorB=84799D&style=flat)](https://github.com/ahmadawais/Emoji-Log/)

pySDPG consists of a set of utilities that collect additional metadata from [SDPG Registry projects](https://digitalpublicgoods.net/digital-public-goods/).

## Table of contents

1. [Getting started](#getting-started)
2. [Project structure](#project-structure)
3. [Docs](#docs)
4. [Contributing](#contributing)
5. [Contributors](#contributors)

## Getting started

### Clone the repo

```
git clone https://github.com/OscarSantosMu/pySDPG.git && cd pySDPG
```

### Create a Python virtual environment

In this example, the Python virtual environment it is called *env* but you could call it differently. If you use a different name make sure you add it to the [.gitignore](.gitignore).

Create it with venv, virtualenv or conda.

<details><summary><b>Show venv instructions</b></summary>

```
python -m venv env
```

where *env* is the name of the virtual environment.
</details>

<details><summary><b>Show virtualenv instructions</b></summary>

```
pip install virtualenv
```
```
virtualenv env
```

where *env* is the name of the virtual environment.
</details>

<details><summary><b>Show conda instructions</b></summary>

```
conda create --no-default-packages --name env
```

where *env* is the name of the virtual environment.
</details>

### Activate the Python virtual environment

From the root of the project (where this README is located)

<details><summary><b>With venv or virtualenv</b></summary>
<details><summary><b>Windows</b></summary>

```
.\env\Scripts\activate
```
where *env* is the name of the virtual environment.
</details>
<details><summary><b>Linux</b></summary>

```
source env/bin/activate
```
where *env* is the name of the virtual environment.
</details>

</details>

<details><summary><b>With conda</b></summary>

```
conda activate ./env
```

where *env* is the name of the virtual environment.
</details>

### Install requirements.txt

```
pip install -r requirements.txt
```

## Project structure

```
src/
├───scripts
├───sdpgairtable
│   └───__init.py__
│   └───module1.py__
│   └───module2.py__
│   └───...
│   └───moduleN.py__
├───sdpgimport
│   └───__init.py__
│   └───module1.py__
│   └───module2.py__
│   └───...
│   └───moduleN.py__
├───sdpglicenses
│   └───__init.py__
│   └───module1.py__
│   └───module2.py__
│   └───...
│   └───moduleN.py__
├───sdpgutilities
│   └───__init.py__
│   └───module1.py__
│   └───module2.py__
│   └───...
│   └───moduleN.py__
└───__init.py__
```

While using pySDPG package without a package manager, scripts must be placed at the src folder, since they use the subpackages (e.g. sdpgairtable). 

For now, all of the Python scripts where placed at the scripts folder to organize the repository and each of them has commented code to execute them without import issues.

When the package is released, there will be no conflicts in finding the modules in the local environment path.


## Docs

To review documentation about the project, follow the steps mentioned in the [Getting started](#getting-started) section and then within the root directory run.

```
pdoc src
```

This command opens a self-hosted server in your machine with the docs.

## Contributing

Please review specific steps, code styling, formatting and conventions in [Contributing.md](CONTRIBUTING.md)

## Contributors

- [Oscar Santos](https://github.com/OscarSantosMu)
- [Ricardo Mirón](https://github.com/ricardomiron)