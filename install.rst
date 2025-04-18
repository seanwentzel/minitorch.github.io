============
Install
============

MiniTorch requires Python 3.7 or higher. To check your version of Python, run either:

>>> python --version
>>> python3 --version


We recommend creating a global MiniTorch workspace directory that you will use
for all modules.

>>> mkdir workspace; cd workspace

We also highly recommand seting up a `virtual
environment`. The virtual environment lets you install packages that
are only used for your assignments and do not impact the rest of the
system. We suggest venv or anaconda.

For example, if you choose venv, run the following command:

>>> python -m venv venv
>>> source venv/bin/activate

The first line should be run only once, whereas the second needs to
be run whenever you open a new terminal to get started for the class.
You can tell if the second line works by checking if your terminal starts
with `(venv)`. See https://docs.python.org/3/library/venv.html for further
instructions on how this works.


Each assignment is distributed through a Git repo. We assume
the knowledge of git throughout the course. See https://guides.github.com
for a tutorial about using git and GitHub.

You should fork the template of the assignment and then edit yours in
your forked repo. Once you have forked the template code, you can
clone your own version by running the following command:

>>> git clone {{ASSIGNMENT}}
>>> cd {{ASSIGNMENT}}


The last step is to install packages.  There are several packages
used throughout these assignments, and you can install them in
your virtual enviroment by running:


>>> python -m pip install -r requirements.txt
>>> python -m pip install -r requirements.extra.txt
>>> python -m pip install -Ue .

Ignore errors on pytest-astropy if shown when installing packages from
requirements.txt.

For anaconda users, you need to run an extra command to install llvmlite:

>>> conda install llvmlite

Make sure that everything is installed by running `python` and then checking:

>>> import minitorch

