# web-fin-finder
[Streamlit](https://docs.streamlit.io/) based web interface app to find and pay fintech talent.


---

## Overview
[Web-fin-finder](app/fintech_finder.py) is an application which allows the user to import Ethereum transaction functions, and sign, execute and inspect transactions.  

---

## Process
[Web-fin-finder](app/fintech_finder.py) will use [python](https://www.python.org/), and highlight the [Streamlit](https://docs.streamlit.io/) web interface library, [web3.py](https://web3py.readthedocs.io/en/stable/) library, and [Ganache](https://trufflesuite.com/ganache/).  

The main web functionality is implemented within [Web-fin-finder](app/fintech_finder.py) and the crypto functionality is imported from [crypto_wallet](/app/crypto_wallet.py).  

**High-level steps:**  
1. Import Ethereum Transaction functions from [crypto_wallet](/app/crypto_wallet.py) into the [application](/app/fintech_finder.py)
2. Sign and execute a Payment Transaction
3. Inspect the transaction in [Ganache](https://trufflesuite.com/ganache/)  

**Submission:**  
- Importing, signing, executing transactions in [fintech_finder.py](/app/fintech_finder.py)
- Screenshots from Ganache showing address, balance history for both sender and receiver.  

## Transaction and Web Application Screenshots

**Address Balance History**
![Address Balance](/media/01_address_balance_hist.png)  

**Transactions**
![Transactions](/media/02_transaction_details.png)  

**Transaction Detail**
![Detail](/media/03_recepient_trans_detail.png)

**Running Web App**
![WebApp](/media/04_web_app.png)  

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

**MNEMONIC ENV VAR**  
You must populate [SAMPLE.env](/app/SAMPLE.env) with your mnemonic words from Ganach application, and then rename the file to `.env` in order for the application to connect to your running Ganache instance and generate an account.

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