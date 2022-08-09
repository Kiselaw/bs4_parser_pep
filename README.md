## Python documentation parser

A simple parser collects various data from Python documentation. 

### Overview

The project is actually a combination of 4 parsers:

- the first one collects links to articles about innovations in Python,
as well as information about the authors and editors of articles.

- the second one collects information about the statuses of Python versions

- the third one downloads an archive with up-to-date documentation

- and finally, the fourth one counts the number of statuses assigned to various PEP's

### Technologies

- Python 3.9.5

### Installation and launch

Clone the repository and go to it using the command line:

```bash
git clone 
```

```bash
cd bs4_parser_pep
```

Create and activate a virtual environment:

Windows:

```bash
py -3 -m venv env
```

```bash
. venv/Scripts/activate 
```

```bash
py -m pip install --upgrade pip
```

macOS/Linux:

```bash
python3 -m venv .venv
```

```bash
source env/bin/activate
```

```bash
python3 -m pip install --upgrade pip
```

Install dependencies from a file requirements.txt:

```bash
pip install -r requirements.txt
```

Launch:

In order to launch you have to use the following commands:

```bash
python arg_parsing.py -h (--help) - shows which commands are allowed
```

```bash
python main.py latest-versions - the first parser
```

```bash
python main.py whats-new - the second parser
```

```bash
python main.py download - the third parser
```

```bash
python main.py pep - the fourth parser
```

Cash  clearing:

```bash
python main.py <command> -c (--clear-cache)
```

Also, there is an optional arguments specifically for latest-versions, whats-new and pep:

```bash
python main.py <command> -o (--output) with pretty or file
```
Depending on the choice, the result is presented either as a "pretty" table or as a csv file.

### License

MIT