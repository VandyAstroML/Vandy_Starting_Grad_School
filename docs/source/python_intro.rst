================================================
Python 101 - Anaconda, environments, and more
================================================

This is a small introduction of what *I* think you should have installed 
in order to property use python in your projects.

--------------------
Anaconda
--------------------

The very first thing for you to have is 
**`Anaconda <https://www.anaconda.com>`_** installed.
From their website:

    With over 4.5 million users, Anaconda is the world’s most popular Python 
    data science platform. Anaconda, Inc. continues to lead open source 
    projects like Anaconda, NumPy and SciPy that form the foundation of 
    modern data science. Anaconda’s flagship product, Anaconda Enterprise, 
    allows organizations to secure, govern, scale and extend Anaconda to 
    deliver actionable insights that drive businesses and industries forward.


Having *Ananconda* installed on your computer is important, since it 
allows you to not worry about installing missing dependencies, 
creates environments for you projects, etc.

^^^^^^^^^^^^^^^^^^^^^
Installing Anaconda
^^^^^^^^^^^^^^^^^^^^^

The first thing is to download Anaconda. If you're starting with 
Python from scratch, it is better to start with **Python 3**.

You can download Anaconda from here: `<https://www.anaconda.com/download>`_, 
and make sure to download the Python 3 version.

.. note:: If you're downloading it from the terminal, you can download the 
    executable from by typing:

    >>> wget https://repo.continuum.io/archive/Anaconda3-5.0.1-MacOSX-x86_64.pkg /path/to/download/to/

    >>> bash /path/to/download/to/Anaconda3*.sh

    For more information on how to download it, go to
    `<https://docs.anaconda.com/anaconda/install/#detailed-installation-information>`_

Once you have downloaded Anaconda, you should be able to start using 
*python* and *iPython*. You can try this by typing the following on the 
terminal:

.. code::

    >>> which python
        /home/username/anaconda/bin/python

    >>> which ipython
        /home/username/anaconda/bin/ipython

    >>> ipython
        Python 3.6.3 |Anaconda custom (64-bit)| (default, Oct  6 2017, 12:04:38)
        Type 'copyright', 'credits' or 'license' for more information
        IPython 6.1.0 -- An enhanced Interactive Python. Type '?' for help.

.. note:: If you're using a separate machine, to which you `ssh`, you can 
    install *Anaconda* to a specified location other than your home directory.
    This is important if you are limited by *the number of files in your 
    home directory**, e.g. a computer hosted by 
    `ACCRE <http://www.accre.vanderbilt.edu/>`_.

^^^^^^^^^^^^^^^^^^^^^^^
Managing environments
^^^^^^^^^^^^^^^^^^^^^^^

When working on a project, it is really important to keep 
**reproducibility** in mind. For example, if you were to hand me you 
code, I should be able to read the documentation and understand it, as 
well as **running the code**.

This is why **creating an environment** for your project is extremely 
important. This is where Ananconda helps a lot. Anaconda let's you have 
your own defined environment for your project, and you can 
**specify which packages** to include in your project.

All of the packages can be specified in an **environment.yml** file.
An example for such file would look like 
(taken from `<conda.io/docs/user-guide/tasks/manage-environments.html>`_):

.. code::

    name: example-environment

    channels:
      - defaults

    dependencies:
      - python=3
      - anaconda
      - astropy
      - h5py
      - numpy
      - pandas
      - scipy
      - seaborn
      - pip
      - pip:
        - GitPython
        - progressbar2
        - halotools
        - sphinx_rtd_theme

You can install the desired environment `example-environment` by 
running the command on the terminal:

>>> conda env create -f environment.yml

For more information, see `<https://conda.io/docs/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file>`_.

.. note:: 
    A helpful package to use is 
    **`conda-env-auto <https://github.com/chdoig/conda-auto-env>`** which allows 
    you to automatically create and *activate* the project environment once you 
    are in the directory. For more information on how to install it and 
    use it, see `<https://github.com/chdoig/conda-auto-env>`_.




