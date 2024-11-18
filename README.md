## Setup

Create a virtual environment (first time only):

```sh
conda create -n reports-env-2024 python=3.10
```

Activate the environment (whenever you come back to this project):

```sh
conda activate reports-env-2024
```

Install packages:

```sh
pip install -r requirements.txt
```

[Obtain an API Key](https://www.alphavantage.co/support/#api-key) from AlphaVantage.

Create a ".env" file and add contents like the following (using your own AlphaVantage API Key):

```sh
# this is the ".env" file:
ALPHAVANTAGE_API_KEY="..."
```

Install packages for email sending:

```sh
pip install -r requirements.txt
```

Obtain an API Key from SendGrid.

Create a ".env" file and add contents like the following (using your own SendGrid API Key):

```sh
SENDGRID_API_KEY = ""
SENDGRID_SENDER_ADDRESS = ""
```

## Usage

Run the example script:

```sh
python app/my_script.py
```

Run the unemployment report:

```sh
#ALPHAVANTAGE_API_KEY="..." python app/unemployment.py

#python app/unemployment.py

python -m app.unemployment
```

Run the stocks report:

```sh
#python app/stocks.py

python -m app.stocks
```

Run the example email sending file:
```sh
python app/email_service.py
```