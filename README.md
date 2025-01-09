# playwright-python-test-automation
This GitHub repository helps you create and build a new test automation project using Playwright in Python.



## Prerequisites
- **VSCode/PyCharm** (code editor)
- **Python 3** (programming language and environment)
- **Playwright** (automation library)



## Installing python
Download and install Python from the following link:
[```https://www.python.org/downloads/```](https://www.python.org/downloads/)

*Note: Install Python as per your operating system(Windows/MAC/Linux)*

### Verify that the python install on your system:

**Linux/macOS:** open a Terminal Window and type the following command: 

```
python3 --version
```

**Windows:** open a command prompt and run the following command:

```
py -3 --version
```



## Setup python in VSCode
After setup Python development environment, add Python extentions in the VSCode.
VS Code Python extensions:
- Python
- Python Debugger
- Pylance



## Clone the repo:

```
git clone "https://github.com/imukesh2508srijan/playwright-python-test-automation.git"

cd playwright-python-test-automation
```



## Create and activate a virtual environment by following command
### For Windows

```
py -m pip install --user virtualenv

py -m venv env

.\env\Scripts\activate
```


### For Mac

```
python3 -m pip install --user virtualenv

python3 -m venv venv

source venv/bin/activate
```


## Install Poetry

```
pip install poetry
```


## To initiate new project use this command:

```
poetry init
```

OR

## To install the current project use this command:

```
poetry install
```


## Add playwright package as dependency:

```
peotry add pytest-playwright

poetry add playwright
```


## Run Tests
To run your tests, use the pytest command. This will run your tests on the Chromium browser by default. Tests run in headless mode by default meaning no browser window will be opened while running the tests and results will be seen in the terminal:

```
pytest
```


### Run tests in headed mode
To run your tests in headed mode, use the --headed flag. This will open up a browser window while running your tests and once finished the browser window will close:

```
pytest --headed
```


### Run tests on different browsers
To specify which browser you would like to run your tests on, use the --browser flag followed by the name of the browser:

```
pytest --browser webkit
```


To specify multiple browsers to run your tests on, use the --browser flag multiple times followed by the name of each browser:

```
pytest --browser webkit --browser firefox
```


### Run specific tests
To run a single test file, pass in the name of the test file that you want to run:

```
pytest test_login.py
```


To run a set of test files, pass in the names of the test files that you want to run:

```
pytest tests/test_todo_page.py tests/test_landing_page.py
```



## Refrences
https://playwright.dev/docs/intro