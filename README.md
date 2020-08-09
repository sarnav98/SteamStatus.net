# SteamStatus.net

Getting Started
Install

git clone https://github.com/akelsch/steamstatus.git && cd steamstatus
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
See requirements.txt for a complete list of required packages.

Configure

steamstatus/config.py:

API_KEY = "" # insert your key here, e.g. 204BE844F017F63E40E2F3D820EB8E9E
UPDATE_FREQUENCY = 60
You can get your own Steam Web API key here.

Run

export FLASK_APP=steamstatus
export FLASK_ENV=development # optional
flask init-db
flask run
Using Windows
PowerShell commands differ quite a bit from Bash so here are some equivalent commands:

# source venv/bin/activate
.\venv\Scripts\Activate.ps1

# export FLASK_APP=steamstatus
$env:FLASK_APP = "steamstatus"

# export FLASK_ENV=development
$env:FLASK_ENV = "development"
Please note that running scripts in PowerShell requires changing your execution policy to Unrestricted (see Set-ExecutionPolicy).
