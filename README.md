![Logo](/app/src/addressio.png)

This project is built with React, and uses a Flask Server as a REST API to store the 
data in a locally stored SQLlite database.

The user can add, edit, and remove people to the address book. They can also add, edit, and remove organisations. 
They are also able to optionally assign each person to an organisation.

![Screenshot](https://user-images.githubusercontent.com/34189022/56148011-501d9480-5fa1-11e9-9a8c-43fcaf48c5ce.PNG)

Here are the steps to getting this up and running. 

### Instructions:

After cloning the repo, you will need to set up both a Flask Server that will be running for the REST API, and you'll need to set up 
a live server for React. You will need to have Python, pip, and npm installed on your PC.

##### Setting up Flask Server:

1. Set up a Python virtual environment in the api folder. Virtual environment
needs to be install with pip. This can be done with:
```
python3 -m pip install --user virtualenv (UNIX)
py -m pip install --user virtualenv (WINDOWS)
```

2. You will then need to create a virtualenv in the Addressio/api directory:
```
python3 -m virtualenv env (UNIX)
py -m virtualenv env (WINDOWS)
```

3. After that is done, you need to activate the virtualenv:
```
source env/bin/activate (UNIX)
.\env\Scripts\activate (WINDOWS)
```

4. After activating the virtual environment, you need to install all the dependancies:
```
pip install -r requirements.txt
```

5. You can then start the server by running this python command:
```
python3 run.py
py run.py
```

##### Setting up React Live Server:

1. Change your directory and go into the Addressio/app directory:
```
npm install 
```

2. After it is done downloading the dependancies and setting up the server, run:
```
npm start
```

And it should be up and running. :)
