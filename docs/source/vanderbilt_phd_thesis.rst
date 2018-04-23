.. _vanderbilt_pdh_thesis:
********************************
Vanderbilt PhD Thesis - Template
********************************

Whenever you're getting close to finishing your Ph.D., you will eventually 
have to start writing up your dissertation. There are many templates 
out there, but there has been one template passed around between  
Astronomy graduate students at Vanderbilt *from generation to generation*.

Now, it's even easier to start writing your dissertation if you 
follow the following steps:

.. _phd_thesis_steps:
========================================
Steps to take to write your dissertation
========================================

The dissertation can be found at: `Vanderbilt Astro PhD Template <https://github.com/VandyAstroML/Vanderbilt_Astro_PhD_Template>`_ 

This template is easy to use, and you only need to answer some questions.

.. _vandy_phd_download:
---------------------------------
Downloading Vanderbilt PhD Thesis
---------------------------------

You first need to run:

.. code-block:: shell
    
    cd /path/to/where/main/thesis/will/be/
    pip install cookiecutter
    cookiecutter https://github.com/VandyAstroML/Vanderbilt_Astro_PhD_Template

This will install the necessary packages and directories for the PhD Thesis.

.. note::

    Make sure you :code:`cd` into the **correct path**. Otherwise, you will 
    be downloading the repository wherever.

.. _vandy_phd_fields:
---------------------------------
Downloading Vanderbilt PhD Thesis
---------------------------------

Next, it will prompt you for some answers.
The different prompts are:

+-------------------------+--------------------------------------------------------------------------+
|Question                 | Description                                                              |
+=========================+==========================================================================+
|:code:`thesis_title`     | Title of the thesis. Should not have '_' symbols in                      |
|                         | it.                                                                      |
|                         |                                                                          |
|                         | Examples:                                                                |
|                         |                                                                          |
|                         | * Understanding Exoplanets and Other Variable Sources                    |
|                         | * The Clustering of Galaxies on the Smallest Scales                      |
|                         |   Across Cosmic Time                                                     |
+-------------------------+--------------------------------------------------------------------------+
|:code:`first_name`       | Author's first name. :code:`first_name` will used                        |
|                         | for the *title page* of the dissertation.                                |
|                         |                                                                          |
|                         | Examples:                                                                |
|                         |                                                                          |
|                         | * Adam                                                                   |
|                         | * Rose                                                                   |
+-------------------------+--------------------------------------------------------------------------+
|:code:`last_name`        | Author's **last** name. :code:`last_name` will used for the *title page* |
|                         | of the dissertation.                                                     |
|                         |                                                                          |
|                         | Examples:                                                                |
|                         |                                                                          |
|                         | * Calderon                                                               |
|                         | * Piscionere                                                             |
+-------------------------+--------------------------------------------------------------------------+
|:code:`repo_name`        | Name of the directory/repository, in which the thesis will be saved.<br> |
|                         | This name is selected by default, but can be changed.<br>                |
|                         | This field **should not contain spaces**.                                |
|                         |                                                                          |
|                         | Examples:                                                                |
|                         |                                                                          |
|                         | * Calderon_Victor_Astro_PhD_Thesis                                       |
|                         | * Szewciw_Adam_Astro_PhD_Thesis                                          |
+-------------------------+--------------------------------------------------------------------------+
|:code:`add_signatures`   | Option for adding signatures to the thesis.                              |
|                         |                                                                          |
|                         | Options:                                                                 |
|                         |                                                                          |
|                         | 1. "y" ... Add signatures                                                |
|                         | 2. "n" ... Do not add signatures                                         |
+-------------------------+--------------------------------------------------------------------------+
|:code:`department_name`  | Name of the department. Default: **Physics and Astronomy**.              |
|                         | Should **not** contain '_' (underscores) symbols.                        |
|                         |                                                                          |
|                         | Examples:                                                                |
|                         |                                                                          |
|                         | * Physics and Astronomy                                                  |
|                         | * Name of another department                                             |
+-------------------------+--------------------------------------------------------------------------+
|:code:`dissertation_date`| Date of the Dissertation presentation.                                   |
|                         | Format: :code:`Month Year`.                                              |
|                         |                                                                          |
|                         | Examples:                                                                |
|                         |                                                                          |
|                         | * May 2019                                                               |
|                         | * August 2020                                                            |
+-------------------------+--------------------------------------------------------------------------+
|:code:`name_committee_1` | First and last name of the committee member 1.                           |
|                         | Should not have '_' symbols in it.                                       |
|                         |                                                                          |
|                         | Examples:                                                                |
|                         |                                                                          |
|                         | * Keivan Stassun                                                         |
|                         | * Andreas Berlind                                                        |
+-------------------------+--------------------------------------------------------------------------+
|:code:`name_committee_2` | First and last name of the committee member 2.                           |
|                         | Should not have '_' symbols in it.                                       |
|                         |                                                                          |
|                         | Examples:                                                                |
|                         |                                                                          |
|                         | * Keivan Stassun                                                         |
|                         | * Andreas Berlind                                                        |
+-------------------------+--------------------------------------------------------------------------+
|:code:`name_committee_3` | First and last name of the committee member 3.                           |
|                         | Should not have '_' symbols in it.                                       |
|                         |                                                                          |
|                         | Examples:                                                                |
|                         |                                                                          |
|                         | * Keivan Stassun                                                         |
|                         | * Andreas Berlind                                                        |
+-------------------------+--------------------------------------------------------------------------+
|:code:`name_committee_4` | First and last name of the committee member 4.                           |
|                         | Should not have '_' symbols in it.                                       |
|                         |                                                                          |
|                         | Examples:                                                                |
|                         |                                                                          |
|                         | * Keivan Stassun                                                         |
|                         | * Andreas Berlind                                                        |
+-------------------------+--------------------------------------------------------------------------+
|:code:`name_committee_5` | First and last name of the committee member 5.                           |
|                         | Should not have '_' symbols in it.                                       |
|                         |                                                                          |
|                         | Examples:                                                                |
|                         |                                                                          |
|                         | * Keivan Stassun                                                         |
|                         | * Andreas Berlind                                                        |
+-------------------------+--------------------------------------------------------------------------+

.. _vandy_phd_writing:
------------------
Writing the Thesis
------------------

Once you've downloaded the repository and answered all of the questions,
you can start writing your thesis.

My advice would be to follow these steps to guarantee that you're doing it 
correctly:

1. Create a new repository on `Github <http://www.google.com>`_.
   This will be the repository for your newly created local repository.
2. :code:`git init` your local repository.
3. Follow the instructions to upload the files of your dissertation to Github.
4. Write your dissertation.


After having downloaded and answered the questions, the repository should look like this:

.. code-block:: shell

    Calderon_Victor_Vanderbilt_Astro_PhD_Thesis/
    ├── Bibliography
    │   └── bibliography.bib
    ├── Chapters
    │   ├── acknowledgments.tex
    │   ├── appendix_A.tex
    │   ├── chapter_1.tex
    │   ├── chapter_2.tex
    │   ├── chapter_3.tex
    │   ├── chapter_4.tex
    │   ├── dedication.tex
    │   ├── future_work.tex
    │   ├── introduction.tex
    │   └── titlepage.tex
    ├── Extras
    │   ├── commands.tex
    │   ├── headings_settings.tex
    │   └── packages.tex
    ├── Figures
    │   ├── project_1
    │   ├── project_2
    │   └── project_3
    ├── Makefile
    ├── README.md
    ├── Thesis
    │   └── thesis.tex
    └── requirements.txt

    8 directories, 18 files

This is the file structure after downloaing the repository.

The main file of the repository is: :code:`Thesis/thesis.tex`.
This is the file that will get compiled by LaTeX, and will produce a PDF 
version.

The only files that you will need to **edit** (aside from :code:`thesis.tex`)
are located in the :code:`Chapters` directory. These are the ones 
that you need to edit.

.. _vandy_phd_compiling:
---------------------
Compiling your Thesis
---------------------

This repository includes a :code:`Makefile`. This file serves as the file 
that will make the *cleaning*, *compiling*, and *opening the pdf* of the
:code:`thesis.tex` file.

To show all of the options of the Makefile, write:

.. code-block:: shell

    make show-help

This will show you a list of options:

.. code-block:: shell

    ./Calderon_Victor_Vanderbilt_Astro_PhD_Thesis: make show-help
    Available rules:

    all                 Perform all tasks
    clean               Clean all unnecessary latex-related files
    open_pdf            List all unnecessary files
    thesis.tex          Compiles Main Thesis file

To compile your thesis, you will need to run the following commands:

.. code-block:: shell

    make thesis.tex

This will create all of the necessary files for compiling your thesis.

To open the PDF version of the thesis, run:

.. code-block:: shell

    make open_pdf

and a PDF version of the :code:`thesis.tex` file will pop up.

.. note::

    In order for properly use the Makefile and compile :code:`thesis.tex`,
    you will need :code:`latexmk` installed. If you're on a MAC, you want 
    to check out `the Latexmk documentation <https://mg.readthedocs.io/latexmk.html>`_,
    and make sure to have `MacTex <https://www.tug.org/mactex/>`_ installed 
    on your computer.

An example of the resulting PDF can be found in: 

.. image:: https://img.shields.io/badge/PDF-Latest-orange.svg
    :target: ./documents/phd_thesis/thesis.pdf
    :alt: Documentation Status










