# Flask_deep_dive

## Flask : The web application framework in Python 

## Installation : Note: make sure you have python 3 and pip preinstalled 

## Installing flask 

### In Mac / Linux 
```
pip3 install flask 
```

### In windows 
```
pip install flask

```

### Sample code --

#### create a file named app.py with the following content 

```
from flask import Flask,render_template
myapp=Flask(__name__)

@myapp.route('/')
def motd():
    return "Hello Flask..!!"


if __name__ == "__main__" :
    myapp.run(debug=True)
```

##  TO RUn the code

### Method 1 

```
fire@XIA:~/Desktop/tech/python_research/flask$ python3 app.py 
 * Serving Flask app 'app' (lazy loading)
 * Environment: production
   WARNING: This is a development server. Do not use it in a production deployment.
   Use a production WSGI server instead.
   
```

### Method 2 

```
fire@XIA:~/Desktop/tech/python_research/flask$ export FLASK_APP=app.py
fire@XIA:~/Desktop/tech/python_research/flask$ flask run
 * Serving Flask app 'app.py' (lazy loading)
 * Environment: production
   WARNING: This is a development server. Do not use it in a production deployment.
   Use a production WSGI server instead.
 * Debug mode: off
 
 ```
 
 
