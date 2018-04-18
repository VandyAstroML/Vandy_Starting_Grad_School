.. _Python_Packaging:
================================================
Python Packaging - Building your own module
================================================

Each project requires its own different functions, definitions, etc.
But most of the times, you will be recycling over old code over and over,
and you will have many duplicates of the same code laying around.

This is why it's important to know how to **build your own python module**.

This is a small tutorial on how to property setup your module, and 
about some of the **very useful** tools that you can use in order to 

- Test your module for errors (Travis CI)
- Keep your documentation up to date (ReadTheDocs)
- and more.

.. _Initial_Setup:
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