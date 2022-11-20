Virtual Environment Configuration:


1.  Installing virtualenv
    virtualenv is used to manage Python packages for different projects. Using virtualenv allows you to avoid installing Python packages globally which could break system tools or other projects. You can install virtualenv using pip.

    $> python3 -m pip install --user virtualenv

2.  Creating Virtual Environment:

    venv (for Python 3) and virtualenv (for Python 2) allow you to manage separate package installations for different projects. They essentially allow you to create a “virtual” isolated Python installation and install packages into that virtual installation. When you switch projects, you can simply create a new virtual environment and not have to worry about breaking the packages installed in the other environments. It is always recommended to use a virtual environment while developing Python applications.

    To create a virtual environment, go to your project’s directory and run venv. If you are using Python 2, replace venv with virtualenv in the below commands.

    $> python3 -m venv env

3.  Activating a virtual environment

    Before you can start installing or using packages in your virtual environment you’ll need to activate it. Activating a virtual environment will put the virtual environment-specific python and pip executables into your shell’s PATH.

    $> source env/bin/activate

4.  Python interpreter confirmation
    You can confirm you’re in the virtual environment by checking the location of your Python interpreter:

    $> which python

5.  Leaving the virtual environment

    $> deactivate

6.  Installing packages

    Now that you’re in your virtual environment you can install packages. Let’s install the Requests library from the Python Package Index (PyPI):

7.  Deleting Virtual Environment
    $> deactivate
    
    # If your virtual environment is in a directory called 'env':
    $> rm -r env
