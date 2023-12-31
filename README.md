# my-first-app-REAL


## Setup

Create and activate a virtual environment: 

```sh
conda create -n my-first-env python=3.10

conda activate my-first-env
```

Install packages

```sh
pip install -r requirements.txt
```

Obtain an [API Key from Alphavantage](https://www.alphavantage.co/support/#api-key) or from the prof (`ALPHAVANTAGE_API_KEY`).

Create a ".env" file and paste in the following contents:

```sh
# this is the ".env" file...

ALPHAVANTAGE_API_KEY="_________"

#You must first follow the [setup instructions](https://github.com/prof-rossetti/intro-to-python/blob/main/notes/python/packages/sendgrid.md) to create an account, verify your account, setup a single sender, and obtain an API Key.

SENDGRID_API_KEY="________"
SENDER_ADDRESS="_______"
```
 
## Usage

Run the example script:

```sh
python app/my_script.py
```

Run the umemployment report:

```sh
#python app/unemployment.py
python -m app.unemployment
```

Send an email:
```sh
python app/email_service.py
```

Run the stocks report:

```sh
python -m app.stocks
```

Run the my_mod.puy file
```sh
python app/my_mod.py
```

#testing

run tests:

```sh
pytest
```

### Web App

Run the web app (then view in the browser at http://localhost:5000/):

```sh
# Mac OS:
FLASK_APP=web_app flask run

# Windows OS:
# ... if `export` doesn't work for you, try `set` instead
# ... or set FLASK_APP variable via ".env" file
export FLASK_APP=web_app
flask run
```