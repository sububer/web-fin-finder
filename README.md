# web-fin-finder
[Streamlit](https://docs.streamlit.io/) based web interface app to find and pay fintech talent.


---

## Overview
Web-fin-finder is an [application](app/fintech_finder.py) which allows the user to import Ethereum transaction functions, and sign, execute and inspect transactions.  

## Assumptions & Process
Web-blockchain applicaton will use [python](https://www.python.org/), and highlight the [Streamlit](https://docs.streamlit.io/) web interface library, [web3.py](https://web3py.readthedocs.io/en/stable/) library, and [Ganache](https://trufflesuite.com/ganache/).  

**High-level steps:**  
1. TBD  

**Submission:**  
- TBD  

## Web Application Testing and Validation

**AppTesting**
TBD  

---

## Technologies

This challenge uses [python](https://www.python.org/) 3.7 and the following modules:  
- [datetime](https://docs.python.org/3.7/library/datetime.html)
- [dateutil](https://dateutil.readthedocs.io/en/stable/)
- [streamlit](https://github.com/streamlit/streamlit)
- [dataclasses](https://docs.python.org/3/library/dataclasses.html)
- [typing](https://docs.python.org/3/library/typing.html)
- [pandas](https://pandas.pydata.org/)
- [hashlib](https://docs.python.org/3/library/hashlib.html)
- [web3.py](https://web3py.readthedocs.io/en/stable/)  

See [installation](#installation) and [usage](#usage) below for specifics.

---

## Installation

You will need Python 3.7, that supports for this application to run. An easy way to install python 3.7 is to download and install [Anaconda](https://www.anaconda.com/products/individual). After installing anaconda, open a terminal/command-prompt, and setup a python 3.7 environment, and then activate it like so:

```
# create an anaconda python 3.7 environment
# name can be any friendly name to refer to your environment, eg 'dev'
conda create --name dev python=3.7 anaconda

# activating the environment
conda activate dev

# use pip to install the above modules, eg:
pip install dateutil
...etc...
```

---

## Usage

To run the application, use the CLI and launch streamlit like:  

```
# activating the environment
conda activate dev

# change to application directory
cd <repo_root>/app

# launch streamlit application
streamlit run fintech_finder.py

```

---

## Contributors

[David Lopez](https://github.com/sububer)

---

## License

MIT