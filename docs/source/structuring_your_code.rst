.. _project_structure_main:

***************************
Structuring your Project
***************************

Now that your have a *working* version of **python** on your computer,
you can start doing research.

One of the key elements of a project is for it to be **reproducible** by 
others. Having this in mind when you're structuring your project will 
allow others to look at your code, understand it well enough to be able 
to **recreate** your results.

This is a short guid on 2 ways to structure your code, without having 
to do much creating of documets, etc.

.. contents:: Table of Contents
    :local:

.. _proj_struc_cookiecutter_sec:

===================================
Cookiecutter and Folder structure
===================================

`Cookiecutter <https://github.com/audreyr/cookiecutter>`_ is a command-line
utility that creates projects from cookiecutters (project templates), 
e.g. Python package projects, LaTeX documents, etc.

Cookiecutter has been widely used for many projects, and each team and 
organization can create their own *template*. For more information,
visit the 
`cookiecutter documentation <https://cookiecutter.readthedocs.io/en/latest/>`_.

As the famous say goes:

.. epigraph::

   Don't reinvent the wheel!

You can always create your own folder and file structures, and organize 
your documents the old-fashioned way. The problem with this is that 
it may **vary** from project to project, and it will be more difficult to 
be consistent and effective throught your projects.

For this reason, I rely on ``cookiecutter`` templates to create the 
file and folder structure of a project.

There are many different ``cookiecutter`` templates out there, but 
after trying to find the best one that suits my needs in **research** and 
**programming**, I found one that works great! And after some modifications,
I came up with a *version* of this template.

These two templates are shown in :ref:`proj_struc_cookiecutter_DS` and 
:ref:`proj_struc_cookiecutter_VC`.

.. _proj_struc_cookiecutter_DS:

----------------------------
Data Science - Cookiecutter 
----------------------------

`Cookiecutter Data Science <https://drivendata.github.io/cookiecutter-data-science/>`_ is best described as

    A logical, reasonably standardized, but flexible project structure for 
    doing and sharing data science work.

This folder structure allows everyone looking at your code to understand 
it right away. It also provides many different functions (as part of a 
``Makefile``) that simplify the workflow of your project.

In a nutshell, this cookiecutter includes:

- A **Makefile** file with **useful functions.
- **Documentation** to make your project easily accessible and readable
- And more!

In order to use this template, you follow the documentation in 
`Cookiecutter Data Science <https://drivendata.github.io/cookiecutter-data-science/>`_.

.. _proj_struc_cookiecutter_VC:

---------------------------------
Personal version - Cookiecutter 
---------------------------------

If you need more than the *normal* Data Science Cookiecutter template, you can 
use my version. Some of the differences are:

- It includes and easy-to-use ``environment.yml`` file that makes it easy to 
  install dependencies.
- Extra functions in the ``Makefile``.
- Choice of what kind of documenation to use. One has the option choose from 
  *traditional* `Read The Docs <https://readthedocs.org/dashboard/>`_ style or 
  the `Astropy Sphinx Theme <https://github.com/astropy/sphinx-astropy>`_.

You can check how these two styles look like:

- |RTD_rtdtheme| - **Read The Docs Version**
- |RTD_astropytheme| - **Astropy Version**

Next, you can create your own Project based on this *cookiecutter* version


.. _proj_struc_cookiecutter_VC_install:

^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Createing your own Project using Cookiecutter
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The first thing to do is to install cookiecutter

.. code-block:: text

    $ pip install cookiecutter

or 

.. code-block:: text

    $ conda config --add channels conda-forge
    $ conda install cookiecutter

""""""""""""""""""""""
To start a new project
""""""""""""""""""""""

To start a new project, type the following:

.. code-block:: text

    $ cookiecutter https://github.com/vcalderon2009/cookiecutter-data-science

If you want the **default** project scheme from *DrivenData* (see above), run:

.. code-block:: text

    cookiecutter https://github.com/drivendata/cookiecutter-data-science

Depending on what kind of folder structure you want, you might want to choose from the different types.

After running this command, **you will be prompted some questions** regarding 
the parameters for the project.

.. Video here!

"""""""""""""""""""""""""""""""""
The resulting directory structure
"""""""""""""""""""""""""""""""""

The directory structure of your new project looks like this:

.. code-block:: text

        ├── LICENSE
        ├── Makefile           <- Makefile with commands like `make data` or `make train`
        ├── README.md          <- The top-level README for developers using this project.
        ├── data
        │   ├── external       <- Data from third party sources.
        │   ├── interim        <- Intermediate data that has been transformed.
        │   ├── processed      <- The final, canonical data sets for modeling.
        │   └── raw            <- The original, immutable data dump.
        │
        ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
        │
        ├── models             <- Trained and serialized models, model predictions, or model summaries
        │
        ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
        │                         the creator's initials, and a short `-` delimited description, e.g.
        │                         `1.0-jqp-initial-data-exploration`.
        │
        ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
        │
        ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
        │   └── figures        <- Generated graphics and figures to be used in reporting
        │
        ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
        │                         generated with `pip freeze > requirements.txt`
        │
        ├── environment.yml    <- The Anaconda environment requirements file for reproducing the analysis environment.
        │                         This file is used by Anaconda to create the project environment.
        │
        ├── src                <- Source code for use in this project.
        │   ├── __init__.py    <- Makes src a Python module
        │   │
        │   ├── data           <- Scripts to download or generate data
        │   │   │
        │   │   └── make_dataset.py
        │   │
        │   ├── features       <- Scripts to turn raw data into features for modeling
        │   │   └── build_features.py
        │   │
        │   ├── models         <- Scripts to train models and then use trained models to make
        │   │   │                 predictions
        │   │   ├── predict_model.py
        │   │   └── train_model.py
        │   │
        │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
        │       └── visualize.py
        │
        └── tox.ini            <- tox file with settings for running tox; see tox.testrun.org


.. _proj_struc_cookiecutter_VC_env:

^^^^^^^^^^^^^^^^^^^^^^^^
Editing your environment
^^^^^^^^^^^^^^^^^^^^^^^^

Now that you have a working proect from **cookiecutter**, you can start by
editing the *environment* of your project.

If you downloaded **my version of cookiecutter**, you should be able to edit 
the ``environment.yml`` file. This file states which packages 
need to be installed by Anaconda and ``pip``  in order to run the 
scripts of the package.

The ``environment.yml`` file looks like the following:

.. code-block:: text

    name: name_of_environment

    channels:
      - defaults

    dependencies:
      - python>=3.6
      - ipython
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

You can edit the ``environment.yml`` file to include/exclude packages 
needed by your project.

After having edited the list of packages needed by your project, you can 
execute the command 

.. code-block:: text

    $ make environment

to **create the environment**.

If you have done this step before, and you want to **update the environment**,
you need to run

.. code-block:: text

    $ make update_environment

instead.


.. _proj_struc_cookiecutter_VC_github:

^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Adding your Project repository it to Github
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If you follow the instructions from above, you should have

* Downloaded the repository
* Created your own project with the desired file and folder structure
* Created your working **environment** for you project

The next step is to add it to `Github <https://github.com/>`_ and make 
it accessible.

To do this, your should do the following:

1. Create a Github repository with the **same name** as the repository.
2. Type ``git add remote origin git@github.com:<username>/<project_name>.git``.
   In here you need to **replace** ``<username>`` and ``project_name`` with 
   your details.
3. ``git push origin master`` - This will push your project to Github.

To check that you did this correctly, type

.. code-block:: text

    git remote -v

and you should get something that looks like this:

.. code-block:: text

    origin  https://github.com/<username>/<project_name>.git (fetch)
    origin  https://github.com/<username>/<project_name>.git (push)

where ``username`` and ``project_name`` pertain to your repository on 
Github.

Now all of the files are online on Github, and should be ready to integrate 
them with `Read The Docs <https://readthedocs.org/>`_.

.. _proj_struc_cookiecutter_VC_RTD:

^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Documentation for your new project 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Now that you have both a working local and online copy of your code, 
the next step is to create the documentation for the project.

For this, you can easily use `Read The Docs <https://readthedocs.org/>`_ (RTD).

You need to do the following:

* Create an account on "Read the Docs"
* Go to your ``Profile`` and select ``My Projects``
* From there, you should import the repository *manually* (it's easier). 
  Click on ``Import a Project`` and follow the instructions.
* You should add the project with the **same name** as the Github Repo if 
  possible. Otherwise, you might need to **change** the links to the *badges*
  on the ``README.md`` files in the project, among others.
* Make sure that the repository was correctly built by looking at the 
  ``Builds`` and see that it compiled correctly. If not, it should tell you 
  if there was an error and what the error was.
* Now you go and change the documentation depending on the project's needs.


.. _proj_struc_cookiecutter_VC_Travis:

^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Continuous Integration for your Project
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Continuous integration** deals with testing your code for possible errors,
and making sure that everything is working as expected. Depending on 
your project's needs.

This template includes a ``.travis.yml``, which the files used by 
`Travis CI <https://travis-ci.org/>`_. Travis CI is a *Continuous integration*
platform for testing your code, and checking the functionality of your
project.

More to come!

.. _proj_struc_links_sec:

===================
Links and Resources
===================

For more information on, you  can take a look at :ref:`Code_Structure_links`
for links and resources on how to structure your code and more.






.. Links

.. |RTD_rtdtheme| image:: https://readthedocs.org/projects/test-cookieproj-rtd/badge/?version=latest
    :target: https://test-cookieproj-rtd.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status

.. |RTD_astropytheme| image:: https://readthedocs.org/projects/test-cookieproj-astropy/badge/?version=latest
    :target: https://test-cookieproj-astropy.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status



