For this course, you need to install Python and a number of scientific Python packages.
We will be teaching using Jupyter notebook, which are ideally suited to interactive Python use, especially when writing accompanying notes.
However, if any attendees have a preference for some other Python environment, such as for example spyder, then they are free to use this.
The code the instructor writes will be written and executed in Jupyter, but this could also be written and executed in other environments.

Instructions below explain how to install Python, Jupyter, and other scientific packages on a Windows or Mac device.
They are many steps involved, which can make the total installation process seem quite demanding.
Fortunately, however, for the purposes of this course, attendess can use Jupyter notebooks online for free using [Google Colab](https://colab.research.google.com/).
This requires no configuration or installation.
See [this introduction](https://colab.research.google.com/notebooks/intro.ipynb) for how Colab works and how to start using it.
This is a great option for anyone who prefers not to immediately install all the software mentioned below.

# Installing Python 

There are many ways to install and set up Python and many ways to use Python. 
I will be following the one that I find the easiest and most reliable and best suited for scientific applications. 
I'll call this the pip-virtualenv-jupyter way.
Other ways of installing and using Python are possible, and I will mention them in the course, but it is best to stick to just one way for a course like this, and I think this is the best way.

In terms of setup, there are around five main steps. These steps are the same on Windows, MacOS, Linux.

1. Install Python 3.9
2. Pip install `virtualenv`
3. Create a virtual environment.
4. Install whatever packages are needed with pip, which can be done at any time from then onwards.
5. Launch jupyter notebook

Below I describe how to do this for Windows and MacOS now. 
Personally, I use Linux, but I won't describe the steps for Linux unless someone wants me to, because I will assume that almost everyone will be using Windows or Macs.

## Windows

### Step 1: Install Python 3.9

Go to https://www.python.org/downloads/ and download the Python 3.9 installer.

Download the `.exe` installer, and then you install that as normal, i.e. double click the installer.
On the opening dialog box, it might give you the option to 'Add Python 3.9 to PATH'. I said yes to this.

Now, open a DOS shell and type `where python`. You should see something like this.

```
C:\Users\psy3andrem> where python
C:\Users\psy3andrem\AppData\Local\Programs\Python\Python39\python.exe
```

The do `where pip` and you should see something like this.

```
C:\Users\psy3andrem> where pip
C:\Users\psy3andrem\AppData\Local\Programs\Python\Python39\Scripts\pip.exe
```

And check the version with `python --version`. You should see something like this.

```
C:\Users\psy3andrem>python --version
Python 3.9.6
```

### Step 2: Install virtualenv

Using the pip installer, install the virtualenv package by typing this command at the DOS command prompt. (The $ indicates the command prompt)

```
$ pip install virtualenv --user
```

### Step 3: Create a virtual environment

You can have as many virtual environments as you want. Each is a separate Python installation. We will create one for this course. We will call it `pyin01_venv`, but we can call it anything we want.

```
$ python -m venv pyin01_venv
```

This will create the virtual environment in the working directory of the DOS session. Unless you change it, it will be your home directory.
Now, we need to activate the virtual environment. You do this

```
$ pyin01_venv\Scripts\activate.bat
```

If that worked, your prompt should now look something like this.

```
(pyin01_venv) C:\Users\psy3andrem>
```

### Step 4: Install packages

Now, we will install some packages. There are tens of thousands to choose from. We will start with some key packages, which we will install with pip.

```
$ pip install jupyter numpy scipy pandas
```

### Step 5: Launch Jupyter

Now we launch a Jupyter notebook.

```
$ jupyter notebook
```

Doing that should open your browser with a Jupyter notebook session. What this is and how to use it is another matter.


## MacOs

### Step 1: Install Python 3.9

Go here https://www.python.org/downloads and get the installer.

Install that as usual on a Mac.

Now, in the Mac's terminal, check the installation. (The $ here means it is is terminal command prompt).

```
$ which python3
/usr/local/bin/python3
```

```
$ which pip3
/usr/local/bin/pip3
```

### Step 2: Install virtualenv

```
$ pip3 install virtualenv --user
```

### Step 3: Create a virtual environment

You can have as many virtual environments as you want. 
Each is a separate Python installation. We will create one for this course. 
We will call it `pyin01_venv`, but we can call it anything we want.

```
$ python3 -m venv pyin01_venv
```

Now activate that virtual environment.

```
$ source pyin01_venv/bin/activate
```

Now your prompt should look something like this.

```
(pyin01_venv) $
```

### Step 4: Install some packages

Now, we will install some packages. There are tens of thousands to choose from. We will start with some key packages, which we will install with pip.

```
$ pip install jupyter numpy scipy pandas
```

### Step 5: Launch Jupyter

Now we launch a Jupyter notebook.

```
$ jupyter notebook
```

Doing that should open your browser with a Jupyter notebook session. What this is and how to use it is another matter.

# Installing additional packages

We can pip install new packages easily now. 

```
pip install seaborn plotnine numba statsmodels rpy2 sympy joblib
```

Note that for `rpy2`, you need to install R (no need for RStudio, just R itself). This can be done as follows:

Go to the [R](https://www.r-project.org/) website and follow the links
for downloading. On Windows, this should lead you to

-   <https://cran.r-project.org/bin/windows/base/>.

Downloading this and following the usual Windows installation process,
you\'ll then have a full working version of R.

On Macs, the installation procedure is essentially identical. The latest
Mac installer should be available at

-   <https://cran.r-project.org/bin/macosx/>.

Download this and follow the usual Mac installation process to get a
full working version of R for Macs.


