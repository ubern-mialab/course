# Installation

## Python Installation

To start with the installation, download the [Anaconda installer](https://www.anaconda.com/distribution/) for your operating system with Python >= 3.8.

### Initial Steps

These steps need to be performed for all operating systems.

1. Create a [Github account](https://github.com/signup?ref\_cta=Sign+up\&ref\_loc=header+logged+out\&ref\_page=%2F\&source=header-home) (The free account is sufficient).
2. Fork the MIA Lab repository:
   1. Go to the MIA Lab repository: [https://github.com/ubern-mialab/mialab](https://github.com/ubern-mialab/mialab)
   2. Fork the repository by clicking on the `Fork` button in the right upper corner.
   3. Follow the instructions on Github.
   4. Go to your MIALab fork (You are at the right location if the text in the left upper corner is of structure `[yourgithubaccount]/mialab`)
   5. Click on the green `Clone` button and copy the URL (https://github.com/\[yourgithubaccount]/mialab.git) shown. You will later use it for cloning your fork to your local machine and probably to [UBELIX](ubelix-hpc.md).

Continue with the operating system specific installation instructions, below.

### Operating System Specific Installation Steps

{% tabs %}
{% tab title="macOS" %}
The installation has not been tested.

**git installation**

Download [git](https://git-scm.com/downloads) and install.

Clone your MIALab repository fork:

```
cd /path/to/where/you/want/the/code
```

Clone the MIALab repository fork using the URL:

```
git clone https://github.com/[yourgithubaccount]/MIALab.git
```

**Anaconda installation**&#x20;

Follow the instructions on the [official website](https://docs.anaconda.com/anaconda/install/mac-os/), and then verify the installation:

```
conda list # which should list all installed Anaconda packages
```

Create a new Python 3.8 environment with the name mialab (confirm with \``` y` `` when promoted during creation)

```
conda create -n mialab python=3.8
```

Activate the environment:

```
conda activate mialab
```

**Install required packages**

```
cd /path/to/MIALab/repository
pip install -r requirements.txt #will install all required packages
```
{% endtab %}

{% tab title="Windows" %}
The installation has been tested on Windows 10.

**git installation**

Download [git](https://git-scm.com/downloads) and install.

Clone your MIALab repository fork - Open "Git Bash"

```
cd \path\to\where\you\want\the\code
```

Clone the MIALab repository fork using the URL:

**Anaconda installation**

Follow the instructions on the [official website](https://docs.anaconda.com/anaconda/install/mac-os/).

Verify the installation - Open "Anaconda Prompt"

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

**Install required packages**

```
cd \path\to\MIALab\repository
pip install -r requirements.txt #will install all required packages
```
{% endtab %}

{% tab title="Linux" %}
Run the following commands in the terminal (tested on Ubuntu 16.04 LTS and 18.04 LTS).

**git installation**

```
sudo apt-get install git
```

Clone your MIALab repository fork:

```
cd \path\to\where\you\want\the\code
```

Clone the MIALab repository fork using the URL:

```
git clone https://github.com/[yourgithubaccount]/MIALab.git
```

**Anaconda installation**

Follow the instructions on the [official website](https://docs.anaconda.com/anaconda/install/mac-os/), and then verify the installation:

```
conda list # which should list all installed Anaconda packages
```

Create a new Python 3.8 environment with the name mialab (confirm with \``` y` `` when promoted during creation)

```
conda create -n mialab python=3.8
```

Activate the environment by

```
conda activate mialab
```

**Install required packages**

```
cd /path/to/MIALab/repository
pip install -r requirements.txt #will install all required packages
```
{% endtab %}
{% endtabs %}

Finally, if all of the above works without issues, test the installation using:&#x20;

Execute the installation test script to verify if all the dependencies are setup correctly.

```
python ./test/test_install.py
```

### Setting up the IDE

Next, move to the [IDE page](ide.md) to setup your favorite development environment to be maximally productive with the code involved with this course!&#x20;

## MATLAB Installation:

Follow the instructions on the [MathWorks website](https://ch.mathworks.com/academia/tah-portal/universitat-bern-40639324.html) to install MATLAB on your computer. Operating System specific requirements are [here](https://ch.mathworks.com/support/requirements/matlab-system-requirements.html). Once you have MATLAB installed, read through the [MATLAB section of the IDE page ](ide.md#matlab)to learn more about working with this program.
