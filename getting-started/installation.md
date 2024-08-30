# Installation

## Installation

To start with the installation, download the [`Anaconda installer`](https://www.anaconda.com/distribution/) for your operating system with Python >= 3.8.

### Initial Steps

These steps need to be performed for all operating systems.

\#. Create a [`Github account`](https://github.com/signup?ref\_cta=Sign+up\&ref\_loc=header+logged+out\&ref\_page=%2F\&source=header-home) (The free account is sufficient).

\#. Fork the MIALab repository

* Go to the `MIALab repository:`[https://github.com/ubern-mialab/mialab](https://github.com/ubern-mialab/mialab)
* Fork the MIALab repository by clicking on the `Fork` button in the right upper corner
* Follow the instructions of Github
* Go to your MIALab fork (You are at the right location if the text in the left upper corner is of structure `[yourgithubaccount]/mialab`)
* Click on the green `Clone` button and copy the URL (`https://github.com/[yourgithubaccount]/mialab.git`) shown. You will later use it for cloning your fork to your local machine and probably to UBELIX.

Continue with the operating system specific installation instructions.

### Operating System Specific Installation Steps

Select your operating system to get the corresponding installation steps:

[**Windows**](#user-content-fn-1)[^1]

The installation has been tested on Windows 10.

git installation

```
  -  Download `git <https://git-scm.com/downloads>`_ and install
```

\#. Clone your MIALab repository fork

```
  -  Open "Git Bash"
  -  :bash:``cd \path\to\where\you\want\the\code``
  -  Clone the MIALab repository fork using the URL from the :ref:`installation_initial_steps_label`
  -  :bash:``git clone https://github.com/[yourgithubaccount]/MIALab.git``
```

\#. Anaconda installation

```
  -  Follow the instructions on the `official website <https://docs.anaconda.com/anaconda/install/windows/>`__
```

\#. Verify the installation

```
  -  Open "Anaconda Prompt"
  -  :bash:``conda list``, which should list all installed Anaconda packages
```

\#. Create a new Python 3.8 environment with the name mialab (confirm with :bash:`y` when promoted during creation)

```
  -  :bash:``conda create -n mialab python=3.8``
```

\#. Activate the environment by

```
  -  :bash:``conda activate mialab``
```

\#. Install all required packages for the MIALab

```
  -  :bash:``cd \path\to\MIALab\repository``
  -  :bash:``pip install -r requirements.txt`` will install all required packages
```

\#. Execute the hello world to verify the installation

```
  -  :bash:``python .\test\test_install.py``
```

**Linux**

Run the following commands in the terminal (tested on Ubuntu 16.04 LTS and 18.04 LTS).

git installation

```
  -  :bash:`sudo apt-get install git`
```

Clone your MIALab repository fork

```
cd /path/to/where/you/want/the/code

# Clone the MIALab repository fork using the URL above

git clone https://github.com/[yourgithubaccount]/MIALab.git
```

Run Anaconda installation script

```
Follow the instructions on the `official website <https://docs.anaconda.com/anaconda/install/linux>`__
No need to install the GUI packages
```

Verify the installation

```
conda list #which should list all installed Anaconda packages
```

Create a new Python 3.8 environment with the name mialab (confirm with :bash:`y` when promoted during creation)

```
conda create -n mialab python=3.8
```

Activate the environment by

```
conda activate mialab
```

Install all required packages for the MIALab

```
  -  :bash:`cd /path/to/MIALab/repository`
  -  :bash:`pip install -r requirements.txt` will install all required packages
```

Execute the hello world to verify the installation

```
  -  :bash:`python ./test/test_install.py`
```

**macOS**

The installation has not been tested.

git installation

```
  -  Download `git <https://git-scm.com/downloads>`_ and install
```

Clone your MIALab repository fork&#x20;

```
cd /path/to/where/you/want/the/code
```

Clone the MIALab repository fork using the URL from the :ref:\`installation\_initial\_steps\_label

```
git clone https://github.com/[yourgithubaccount]/MIALab.git
```

Anaconda installation&#x20;

Follow the instructions on the [`official website`](https://docs.anaconda.com/anaconda/install/mac-os/)

Verify the installation

```
conda list # which should list all installed Anaconda packages
```

Create a new Python 3.8 environment with the name mialab (confirm with :bash:`y` when promoted during creation)

```
conda create -n mialab python=3.8
```

Activate the environment by

```
conda activate mialab
```

Install all required packages for the MIALab

```
cd /path/to/MIALab/repository
pip install -r requirements.txt #will install all required packages
```

Execute the installation test script to verify if all the dependencies are setup correctly.

```
python ./test/test_install.py
```

[^1]: 
