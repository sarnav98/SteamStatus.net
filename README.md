<h1 style="text-align:center;">SteamStatus.net</h1>

<h2 style="text-align:center;">Install</h2>
<ul>
<li>git clone https://github.com/sarnav98/SteamStatus.net.git</li>
  <li>cd SteamStatus.net</li>
  <li>python -m venv venv</li>
  <li>source venv/bin/activate (For MacOS Users)</li>
  <li>.\venv\Scripts\Activate.ps1 (for Windows users)</li>
  <li>pip install -r requirements.txt</li>
</ul>
<br>
<h2>Configuration of the Flask</h2>
<br>
<ul>
<li>Open config.py and update Steam API key</li>
<br>
<p>EXAMPLE: API_KEY = "" # insert your key here, e.g. 204BE844F017F63E40E2F3D820EB8E9E</p>
</ul>
<br>
<h2 style="text-align:center;">Run</h2>
<ul>
  <li>export FLASK_APP=steamstatus (For MacOS)</li>
  <li>$env:FLASK_APP = "steamstatus" (For Windows PowerShell)</li>
  <li>export FLASK_ENV=development # optional (for MacOS)</li>
  <li>$env:FLASK_ENV = "development" (For Windows PowerShell)</li>
  <li>flask init-db</li>
  <li>flask run</li>
</ul>
<br>
<p>Please note that running scripts in PowerShell requires changing your execution policy to Unrestricted (see Set-ExecutionPolicy).</p>
<p>Write the following command in PowerShell before executing any of the code above - <b>set-executionpolicy remotesigned</b></p>
