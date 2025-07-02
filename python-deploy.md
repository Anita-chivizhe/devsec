from flask import Flask, jsonify

from flask_cors import CORS

app = Flask(**name**)

CORS(app)

@app.route('/api/message')

def message():

    return jsonify({"message": "Hello from Ubuntu EC2!"})

if **name** == "**main**":

    app.run(host="0.0.0.0", port=5000)

sudo apt update -y

sudo apt install python3-pip -y

python3 --version

pip3 --version

sudo apt install python3-venv -y

python3 -m venv venv

# activate it

source venv/bin/activate

# confirm

which python

which pip

# now install

pip install flask flask-cors
