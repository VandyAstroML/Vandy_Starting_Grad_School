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

You first need to run:

.. code-block:: shell
    
    cd /path/to/where/main/thesis/will/be/
    pip install cookiecutter
    cookiecutter https://github.com/VandyAstroML/Vanderbilt_Astro_PhD_Template

This will install the necessary packages and directories for the PhD Thesis.

.. note::

    Make sure you :code:`cd` into the **correct path**. Otherwise, you will 
    be downloading the repository wherever.

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
|:code:`repo_name`        | Name of the directory/repository, in which the thesis will be saved.     |
|                         | This name is selected by default, but can be changed.                    |
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











