.. _Python_Packaging_sec:
==========================================================
Python Packaging - Building your own module and package
==========================================================

.. contents:: Table of Contents
    :local:

.. _Packaging_Intro_sec:
-----------------------
Introduction
-----------------------

Each project requires its own different functions, definitions, etc.
But most of the times, you will be recycling over old code, over and over,
and you will have many duplicates of the same code laying around.

This is why it's important to know how to **build your own python module**.

This is a small tutorial on how to property setup your module, and 
about some of the **very useful** tools that you can use in order to 

- Test your module for errors (Travis CI)
- Keep your documentation up to date (ReadTheDocs)
- and more.

.. _Initial_Setup_sec:
---------------------------------
Initial Setup
---------------------------------

In order to construct your package, you first need to setup your package 
with the following folder structure:

.. code::

    your_package/
        LICENSE.txt
        README.txt
        setup.py
        package_name/
            __init__.py

As you can tell, there's a file named :code:`__index__.py`. This file tells 
Python to treat this directory as a *module/package*. Without 
this file, Python will not understand that your building a package, and 
will not link the files properly.

There are many different ways to create a Python module.
I prefer to use `cookiecutter <https://github.com/audreyr/cookiecutter>`_.
Cookiecutter is a command-line utility that creates projects from cookiecutters
(project templates), e.g. creating Python package project from a Python 
package project template. For more information on cookiecutter, see 
`https://github.com/audreyr/cookiecutter <https://github.com/audreyr/cookiecutter>`_ .

For creating a Python project, there are different methods.
But I prefer these two methods:

* `Astropy Template <https://github.com/astropy/package-template>`
* `PyPackage <https://cookiecutter-pypackage.readthedocs.io/en/latest/>`_

Depending on what kind of package you intend to produce, the Astropy 
Template or PyPackage should be enough for creating a new Python package.


.. _Astropy_Template_sec:
^^^^^^^^^^^^^^^^
Astropy Template
^^^^^^^^^^^^^^^^

This template is powered by the `Astropy Project <http://www.astropy.org/>`_.
After answering a few questions, this project will create the folder structure
for your new Python Package.

.. _Astropy_Template_install_subsec:
"""""""""""""""""""""""""""
Installing Astropy Package
"""""""""""""""""""""""""""

To first install the Astropy Template, you need to run::

    conda install -c conda-forge cookiecutter gitpython

or::

    pip install cookiecutter gitpython

This will instal the necessary dependencies of ``cookiecutter``. Now 
you can go ahead and run the following commands to create the structure of 
your Python package::

    cd /path/to/new/Python/Package
    cookiecutter -c cookiecutter gh:astropy/package-template

This will prompt you with a series of questions about your project.
For a full list of the different options during Setup, see 
`Options during Setup <http://docs.astropy.org/projects/package-template/en/latest/options.html#options>`_.

.. _Astropy_Template_continous_integrations_subsec:
""""""""""""""""""""""""""""""""
Setting up Continuos Integration
""""""""""""""""""""""""""""""""

After having created the folder structure of the new Python structure,
it is advisable to use continous integration to ensure that all of the 
modules and functions are behaving the way they are supposed to.

The ``Astropy Template`` comes with easy-to-use files that you can modify 
to use with `Travis CI <https://travis-ci.org/>`_ and other CI clients.

For more information on CIs and how to use them, see 
`Setting up Continous Integration <http://docs.astropy.org/projects/package-template/en/latest/nextsteps.html#setting-up-continuous-integration>`_ .

.. _Astropy_Template_rtd_subsec:
""""""""""""""""""""""""""""""""
Documentation and Read the Docs
""""""""""""""""""""""""""""""""


.. _PyPackage_sec:
^^^^^^^^^^^^^^^^^^
PyPackage Template
^^^^^^^^^^^^^^^^^^



.. _Resources_sec:
------------------------------------
Resources and further reading
------------------------------------

This is a small list for further reading

- `The Hitchhiker’s Guide to Packaging <https://the-hitchhikers-guide-to-packaging.readthedocs.io>`_
- `Python Packaging User Guide <https://packaging.python.org/>`_
- `Astropy Package Template <http://docs.astropy.org/projects/package-template>`_

