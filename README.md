# recurse-quiz-app

## Table of Contents 

- [Installation](#installation)
- [Notes over structure](#notes-over-structure)
- [Common Issues](#common-issues)



## Installation
1. Install python & pipenv
  - pip installation might be required as well

2. To enter the virtual environment
    ```shell
    pipenv shell
    ```

3. To install the required dependencies:
    ```shell
    pipenv install -r requirements.txt
    ```

```TODO: Add commands for upgrading the database & seeding```

4. Create a .env file in the recurse-quiz-app directory and enter this on the first line
    ```shell
   SECRET_KEY=randomcharacters
    ```
4. To start the server use command line:
    ```shell
    python wsgi.py
    ```

## Notes over structure

![Example Image](./web-quiz-plan.png)



## Common Issues

In case of Pylance import errors on VSCode, try:
1. Run:
    - Open the command palette
    - Go to Python Clear Cache and Reload
2. Run:
    - pipenv --venv
    - Open the command palette
    - Go to Python Select Interpreter
    - Then manually enter the interpreter path as the Python interpreter
    - This is in the command palette on VSCode

The above is also true for if Pycharm notifies you that there is no python interpreter configured! To solve via the Pycharm GUI:

1. Get the location of your pipenv virtual environment by running 'pipenv --venv'
2. Click configure python interpreter
3. Click add New interpreter
4. Click add local interpreter
5. Click the 'Existing' radio buton, then the ... icon.
6. Paste the location of the pipenv virtual environment
7. Look for the bin folder to your corresponding virtual environment
8. Select the file which corresponds to your version of python (for this case, python3.9) and hit OK
