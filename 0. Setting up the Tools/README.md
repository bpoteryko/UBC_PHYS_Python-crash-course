# 0. Setting Up the Tools
We are going to need multiple tools for the workshop. This module guides you through installing all of them. Do not worry if you do not understand all the following steps and concepts. You will get familiar with it soon enough.

## Installing Anaconda
Anaconda is a package manager (a program that helps you install all the things you need, and that keeps it organized) which is made for Python. To install Anaconda, do the following:

- Download the _Python 3.7 version_ installer suitable for your operating system from https://www.anaconda.com/download/
  - If you are using a Windows computer, you will need to know if your computer is built on a 32-bit or 64-bit architecture. You can find this in the _About your PC_ section of _System Settings_. If you are uncertain how to find this, you can follow [these instructions](https://support.wdc.com/knowledgebase/answer.aspx?ID=9405).
  - If you are using a Mac made after 2007 you will have a 64-bit architecture.
- Run the installer.

## Setting up a virtual environment
Different projects might need to use different versions of Python. We will, therefore, set up a "virtual environment" that we can use for executing Python code. This will also enable us to access the packages we want and ensure they do not conflict.
- Launch `Anaconda-Navigator`
  - you will find the Anaconda-Navigator in launchpad in macOS and in the start menu in Windows.
- Go to the _Environments_ tab on the left-hand side of the screen.

![](Images/Anaconda0.png)

- Click the _Create_ button at the bottom of the screen.
- The dialogue seen in the following figure will appear:
  - Give the environment a name of your choosing (for example `phys_py37`).
  - Select the check-box for Python and select 3.7 from the dropdown. This is the version of Python we are going to use.
  - Ensure R is unchecked. R is an entirely separate programming language focussed on statistics applications.
  - Select _Create_.

![](Images/Anaconda1.png)

You have now made your own environment. It may appear below your "base (root)" environment which is the global environment on your computer. Other applications may be using this global environment, so if we install packages here, problems may arise. By keeping a separate virtual environment, you ensure this does not happen.

## Installing packages
The functionality of programming languages is often separated into libraries. In Python, these libraries are called _packages_ that we can download and access to make our work easier.

### Using the Conda package manager
The package manager in Anaconda is called Conda. We can now install the packages we need in our newly made environment using Conda. Do as follows:
- Ensure the environment we just created is active.
  - It should be highlighted in the _Environemnts_ inspector as seen in the picture below.
  - If it is not active, click on the environment to activate it. Changing environments can take some seconds, so be patient.

![](Images/Anaconda2.png)

- Select _Not installed_ from the dropdown to show all the packages Anaconda knows about that are not installed in your environment already.
- Search for `matplotlib`. When it appears, select the checkbox for the package and hit _Apply_.

![](Images/Anaconda3.png)

- Select _Apply_ in the dialogue that appears to confirm the installation of the dependencies, and wait until the package is installed.
- You can also install `scipy` in the same way as we will need it towards the end of the week.

### Using the _pip_ package manager
We are going to use a package called `Arduino-Python3` a lot as we progress in the course. This package is not available through the package manager in Anaconda. To install it, we need to use another package manager called _pip_. It works well together with Conda.

To install `Arduino-Python3` with _pip_, do the following:
 - Go to the environments tab of Anaconda.
 - Click the play button next to the Python environment you set up earlier.
 - Click _Open Terminal_.

You will get a Terminal/Command Line window which is referencing the Conda environment you launched it from.
 - Type `pip install arduino-python3` followed by return.
 - _pip_ will set to work and give you a message indicating if the installation was successful.
   - If the package was successfully installed, close the Terminal/Command Line window and return to Anaconda.
   - If you encountered an error, ask for help.

After having installed the package, my terminal window looks like this:
![](Images/terminal.png)

## Getting started with Spyder
Spyder is a scientific Python development environment that makes it easy to write and run Python code.

### Installation
 You can install it from within Anaconda as follows:
- Go to the _Home_ tab on the upper left side of the Anaconda window.
- Ensure the _Applications on_ dropdown on the top of the screen is set to the environment `phys_py37` that we just created.
- Find Spyder and click _Install_. Wait until the installation is completed.

![](Images/Anaconda4.png)

### Use
To start working with Spyder, do the following:
- Again, ensure the _Applications on_ dropdown on the top of the screen is set to the environment `phys_py37` that we just created (or whichever environment you want to run code in).
- Hit "Launch" on Spyder.
- You are now greeted with the Spyder interface. It consists of three parts:
  - Code editor: where you write your Python code
  - Directory: where you store and access your files
  - Console: where you run and view the output from your code

![](Images/Spyder1.png)

- After you have written some code you want to run, click the green play button at the top of the screen.
- Set the directory path (circled in the picture above) to where you want your code to be saved.



You have now got all you need to start writing Python! Go to the next module to continue.

Next: [Module 1: Learning Python](/1.%20Learning%20Python/)
