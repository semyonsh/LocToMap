# LocToMap

A PoC to display DNS LOC records on a map. It uses fastapi to serve a minimal api which responds to domains. A static map file is served from the root from where domains can be entered

Give it a spin, try ```SW1A2AA.find.me.uk``` for example

Some more information on the LOC record
https://en.wikipedia.org/wiki/LOC_record
https://www.rfc-editor.org/rfc/rfc1876.html


# Running it

Create a new virtualenv

```shell
python -m venv venv
```

Load the virtualenv and pull in the requirements

```shell
# Linux
source venv/bin/activate
# Windows
.\venv\Scripts\activate

pip install -r requirements.txt
```

Run the app with uvicorn

```shell
uvicorn main:app --reload
```
