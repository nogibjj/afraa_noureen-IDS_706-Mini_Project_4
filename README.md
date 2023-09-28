# IDS_706-Data_Engineering_Systems
## Mini-Project 4 : GitHub Actions Matrix Build for Multiple Python Versions

[![CI](https://github.com/nogibjj/afraa_noureen-IDS_706-Mini_Project_4/actions/workflows/cicd.yml/badge.svg)](https://github.com/nogibjj/afraa_noureen-IDS_706-Mini_Project_4/actions/workflows/cicd.yml)

***

#### Purpose
This repo is for Mini-Project 4 of the Data Engineering course. The purpose is to establish a GitHub Actions workflow designed to facilitate the systematic testing of the codebase against different Python versions.

The fundamental project requirements are as follows:
1. Implementation of a GitHub Actions workflow.
2. Ensuring the testing of the codebase across a minimum of three different Python versions.

To streamline the integration of the codebase into the development pipeline, I configured the GitHub Actions Matrix Build to trigger automatically upon each instance of code push or pull request directed towards the main branch. This configuration guarantees testing across the different Python versions, spanning both the Ubuntu and Windows operating systems.

***

#### This template includes:
1. **.devcontainer**: configuration folder which contains a **Dockerfile** and **devcontainer.json**.
   - **Dockerfile**: specifies the instructions for building a Docker container image that will be used as the development environment.
   - **devcontainer.json**: defines the settings for the development container, such as which Dockerfile to use and environment variables.
3. **Makefile**: contains a set of rules that define how to compile source code, run tests, and perform other development tasks. 
4. **requirements.txt**: lists all the external libraries and dependencies required for the project to run correctly. It helps ensure that everyone working on the project uses the same versions of libraries, which is important for reproducibility and compatibility.
5. **workflows**: contains configuration file **(cicd.yml)** for matrix build that tests more than one version of Python.
6. **main.py**: contains a basic function which displays system info.
7. **test_main.py**: python file to test the function in main.
8. **README**: gives developers a detailed description of the GitHub project.
9. **.gitignore**: specifies files and directories that should be ignored by Git, the version control system used by GitHub. Changes in files or directories in the .gitignore file will not be tracked by Git, and they will not be included in the version history.

***

### Commands to Run the Repo

To run the project, you can use the Makefile and follow these commands:
1. ```
   # To install the required the python packages
   make install
   ```
2. ```
   # To check code style
   make lint
   ```
3. ```
   # To run tests
   make test
   ```
4. ```
   # To format the code
   make format
   ```
5. ```
   # To perform all the above tasks (install, test, format, lint)
   make all
   ```

***

### Result

1. On running ```make lint```:

![lint](https://github.com/nogibjj/afraa_noureen-IDS_706-Mini_Project_4/assets/143756865/d9640421-9adb-4e8d-ad2b-2cd2fa3ca501)

2. On running ```make test```, it passes the test:

![test](https://github.com/nogibjj/afraa_noureen-IDS_706-Mini_Project_4/assets/143756865/6848df7a-c929-41e1-93ae-3f8906282f40)

3. On running ```make format```:

![format](https://github.com/nogibjj/afraa_noureen-IDS_706-Mini_Project_4/assets/143756865/f5cfc452-db98-4f24-9539-166d3d3cddf4)

***

### Successful Workflow Run

![workflow](https://github.com/nogibjj/afraa_noureen-IDS_706-Mini_Project_4/assets/143756865/1a6b2a5c-5a5e-4135-8036-6751481baf57)
