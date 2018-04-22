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

+---------------------+--------------------------------------------------------------------------+
|Question             | Description                                                              |
+=====================+==========================================================================+
|:code:`thesis_title` | Title of the thesis. Should not have '_' symbols in it.                  |
|                     | Examples:                                                                |
|                     |                                                                          |
|                     | * 'Understanding Exoplanets and Other Variable Sources'                  |
|                     | * 'The Clustering of Galaxies on the Smallest Scales Across Cosmic Time' |
+---------------------+--------------------------------------------------------------------------+
|:code:`Ctrl-a k`     | Kill the current window                                                  |
+---------------------+--------------------------------------------------------------------------+

.. {
..     "thesis_title" : "Thesis Title",
..     "first_name" : "firstname",
..     "last_name" : "lastname",
..     "repo_name" : "{{ cookiecutter.last_name + '_' + cookiecutter.first_name + '_Vanderbilt_Astro_PhD_Thesis' }}",
..     "add_signatures" : ["y","n"],
..     "department_name" : "Physics and Astronomy",
..     "dissertation_date" : "May 2019",
..     "name_committee_1" : "Member1",
..     "name_committee_2" : "Member2",
..     "name_committee_3" : "Member3",
..     "name_committee_4" : "Member4",
..     "name_committee_5" : "Member5",
..     "_copy_without_render" : [
..         "Extras/headings_settings.tex",
..         "Extras/commands",
..         "Extras/packages"]
.. }










