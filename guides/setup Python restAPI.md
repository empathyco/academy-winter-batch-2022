# Setup flask python rest API
## Contents:
* Setup a virtual environment
* Update pip and install dependencies
* Use the virtual environment in vsCode
* Setup with Conda
* Create api.py file
* Setup Dockerfile and docker-compose
* Enjoy
&nbsp;

## Author
- [Marcos Tobias](https://github.com/MarcosTobias)
&nbsp;


## Setup a virtual environment
First, install venv:
```
python3 -m venv <path>
```
Where path is the location you want the venv to be created (I use a folder in ~/Documents)
Then,
````
source <path>/bin/activate
````
Now the terminal should be activated. You know it is if there is (\<path\>) written before each line on the terminal.
For deactivating it, run:
````
deactivate
````
&nbsp;

## Update pip and install dependencies
Run: 
````
pip install --upgrade pip
````
Now, for installing the packages (These are just the neccesary packages for the restAPI, you would need to install every package needed for running your scripts too) I recommend installing them one by one, pip is a little picky if you try to install them all at the same time.
````
pip install flask
pip install flask_cors
pip install flask_restx
pip install numpy
pip install pandas
````
Now for saving the libraries needed for running the app:
````
pip freeze > requeriments.txt
````
You would need to run this command every time you install a new library on the virtual environment.

&nbsp;

## Use the virtual environment in VSCode
Open VSCode, and go to settings. Write venv and on the "Python: venv path" write the absolute path of the venv installed on the first step. It would look something like this:
````
~/Documents/<path>
````

Reset VSCode. For using our virtual environment there are different ways. The first one would be pressing cmd + shift + p, and writing "Interpreter". Click on the "Python: Select interpreter", and select the path for the virtual environment, it should appear there. If it does not appear, add it on the first option and restart VSCode again.

Another option would be to create an api.py file, and opening it. Now on the bottom right corner of VSCode should appear the python version. Clicking on it would open a dialog for changing the interpreter as well.

Now open a terminal, ctrl + shift + `, and it should also have (\<path\>) at the beginning of each line. If you had a previous terminal opened before changing the interpreter, you may need to close and open again the terminal for it to be displayed.

&nbsp;

## Setup with conda
If you have conda and want to use it, the steps are the following:
````
conda create --name myenv
conda activate myenv
````

Now, open VSCode and press cmd + shift + p, and write interpreter. Click on select python interpreter, and on the list should appear myenv, the new virtual environment we just created. If it does not appear, close and open it again.
Then, open a terminal with control + shift + `, and myenv should appear on the beggining of each line.

Run on the terminal:
````
conda install pip
````
And now you can follow the steps in "Update pip and install dependencies", and skip to "Create api.py file".

&nbsp;

## Create api.py file
The basics contents of this file should be:
````
from flask import Flask, jsonify
from flask_cors import CORS
from flask_restx import Resource, Api


app = Flask(__name__)
CORS(app)
api = Api(app, version='1.0', title='Sample text', description='Sample text 2')

@api.route('/status')
class Status(Resource):
    @api.response(200, 'Success')
    @api.response(500, 'Internal Server Error')
    def get(self):
        return jsonify({'status': 'healthy'})

if __name__ == '__main__':
    app.run(debug=True, host='0.0.0.0', port=5000)
````
This is enough for a basic api. You can run it from the terminal with:
````
python api.py
````
And for checking if it works, run in a terminal:
````
curl localhost:5000/status
````
If you open it in a browser you can see the Swagger documentation at:
````
localhost:5000
````
&nbsp;

## Setup Dockerfile and docker-compose
Now create the Dockerfile with this contents:
````
# syntax=docker/dockerfile:1
FROM python:3.9-slim-buster

WORKDIR /restapi

COPY requeriments.txt requeriments.txt

RUN pip3 install -r requeriments.txt

RUN apt-get update

COPY . .

CMD ["python", "api.py"]
````

And a docker-compose.yml file with:
````
version: '3.5'
services:
  restapi:
    container_name: "flaskRestAPI"
    build: .
    ports:
    - "5000:5000"
````

You need to have Docker installed and running, and for launching the API now run in a terminal:
````
docker-compose up --build -d
````

And as before, you can check that the api is working correctly with:
````
curl localhost:5000/status
````


