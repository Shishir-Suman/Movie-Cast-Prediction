COLLABORATORS FOR PROJECT UPDATED
John Abraham, Terence Au, Shishir Suman, Daniel Zagyva, Cinmay Palande, Nitish Kholgade

DESCRIPTION

This package contains an html file, files for the web app using the flask python
and a toy data set to be used for demonstration.  After the setup, opening the
html file will open an interactive web app where the user can recieve cast
reccomendations for their movie; more details on using the interface is in the
demo section of this readme.

BROWSER COMPATIBILITY: Firefox

INSTALLATION:
this section describes how to install the server files as a python package.

1)  Install python 3.5

--------------------------------------------------------------------------------
2)  Create virtual python environment and activate it: either make one in using
    Anaconda (easiest) or download the virtualenv python package.

Using Anaconda:
    -Open the anaconda terminal
    -Run the command: conda create  --name <name here>  python=3.5
    -From the anaconda terminal, run the command  for windows:  activate
    <name of environment>.  For mac or LINUX: source activate <name of environment>

Using the virtualenv package:
    -Install the virtualenv python packge if it is not already installed on your
     machine.
        -Open command prompt/terminal
        -Run command:  pip install virtualenv to install package
    -Run the command : virtualenv <installation directory here>
    -Change to the virtual environment directory just created and navigate to
     the  “Scripts” folder within.
    -Run the appropriate activation script depending on your OS. Either
     activate.bat or activate.ps

--------------------------------------------------------------------------------
3)  Now that the virtual environment is activated, navigate to the
    movies_backend/movies_backend directory in the installed folder.

--------------------------------------------------------------------------------
4)  Install required python packages: run the following command:
    pip install –r requirements.txt

    Note: there may be a notification about deprecated packages but the package
    will still run

--------------------------------------------------------------------------------
5) to start the server run the following command: python movies_backend.py

Once you see the following line in the terminal the python server is running:

* Running on http://127.0.0.1:5000/

6)  The python server is now setup and running. procede to the EXECUTION
    section to run the tool.

================================================================================

EXECUTION
The following section describes how to run a demonstration of the tool

0) Make sure the python server is running (see step 5 in the previous section).

1) navigate to the Viz v1.0 folder from the top level of the installation
   dirctory. Open the viz.html file USING FIREFOX browser.  The tool is not
   supported in other browsers.

2) Once the tool has loaded, find the "director" text box type a name.

3) Select three movie genres from the "genres" dropdown boxes.

4) Select the number of actors to be cast from the "Number of Actors" dropdown
   box.

5) Enter a short synopsis of the movie in the "Synopis" text box and click the
   "Initialize"  button.

6) Select the age, gender, and popularity of the first actor in the column
   labeled "Actor 1" and click the "Recommend" button.  The tool will take a few
   seconds to process the request.

7) Once the tool has finished processesing an alert will show. Dismiss the alert
   and hover the mouse over the pictures of each actor; a tooltip will display
   more information about that actor.

8) Click on an actor's picture to select them as your cast member.

9) Repeat steps 6-8 for however many other actors you chose to cast.

NOTES: -actors must be selected in order from left to right.  A popup will
        remind you if you try to make a selection out of order
       -to make sure the model is making recommendations based on the most
       recent inputs, the window resets whenever a dropdown box with information
       from a previous actor is changed. Simply click the "Initialize" button
       to show the actor columns again.
       - if there is an installation error with the following error code:

       "python setup.py egg_info" failed with error code 1

        update setuptools with the following line:
        pip install --upgrade setuptools
