## Ubuntu link
[https://drive.google.com/drive/u/0/folders/1me_nJJh0fvdDOXX3ew2jzGQpoP7f_iFt]()

## C compiler commands
```
sudo apt update
sudo apt install build-essential // sudo apt install gcc
```

## scp command
```
scp filename.txt username@ip_address:/home/username
```
## Google Cloud App Engine
```
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt

main.py
import flask

app = flask.Flask(__name__)

@app.get("/")
def hello():
    return "Hello World!\n"

if __name__ == "__main__":
    app.run(host="localhost", port=8080, debug=True)

requirements.txt
Flask==3.0.2

app.yaml
runtime: python312

gcloud app deploy

documentation
[https://codelabs.developers.google.com/codelabs/cloud-app-engine-python3#0]()
```
