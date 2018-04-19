.. _useful_tools:
*********************************
Tools you might want to check out
*********************************

.. contents:: Table of Contents
    :local:

.. _tools_intro:
============
Introduction
============

There are tools out there that can make your workflow **much, much smoother**.
This is a small list of some of the tools that I've found useful throughout my 
stay at Vanderbilt. They have significantly improved my workflow, and 
have made the projects much easier to understand.

.. _htop_sec:
=====================================
htop - An interactive viewer for Unix
=====================================

For viewing which processes are running on your computer and how much 
memory is left, I like to use `htop <https://hisham.hm/htop/>`_.

This application, as shown in 

.. _Fig-1.1:
.. figure:: ./images/useful_tools/htop.png
    :alt: htop running in the terminal

    Figure 1.1: htop running in the terminal.
    Credit: `Wikipedia <https://en.wikipedia.org/wiki/Htop#/media/File:Htop.png>`_

This tools is extremely useful when running multiple jobs, since it lets 
you see which *jobs* are running, for how long they've been running, and 
more. Figure :numref:`Fig-1.1` how *htop* looks whenever you run this 
from the terminal:

.. code-block:: shell

    htop

.. _htop_explained:
--------------
htop Explained
--------------

htop has different things to offer. Figures :ref:`Fig-1.2` and 
:ref:`Fig-1.3` explain what each column means.

.. _Fig-1.2:
.. figure:: ./images/useful_tools/htop_top.png

   Top of *htop*. This figure shows the different components in the 
   upper part of *htop*.
   Credit: `CodeAhoy <https://codeahoy.com>`_

And the bottom part ...

.. _Fig-1.3:
.. figure:: ./images/useful_tools/htop_bottom.png

   Top of *htop*. This figure shows the different components in the 
   bottom part of *htop*.
   Credit: `CodeAhoy <https://codeahoy.com>`_


.. _htop_resources:
---------------
Further Reading
---------------

For a **more in depth discussion** of the different sections of :code:`htop`, 
see:

* `htop Explained Visually <https://codeahoy.com/2017/01/20/hhtop-explained-visually/>`_
* `Understanding and using htop monitor system resources <http://www.deonsworld.co.za/2012/12/20/understanding-and-using-htop-monitor-system-resources/>`_
* `htop Explained <https://peteris.rocks/blog/htop/>`_

.. _tmux_screen_sec:
=============================================
tmux and screen - Terminal Multiplexers
=============================================

Two other great tools that you should get familiar with are:

* :code:`screen` - `GNU Screen <https://www.gnu.org/software/screen/>`_ 
* :code:`tmux` - `Github Tmux <https://github.com/tmux/tmux>`_ 

These two tools are essential when working on the terminal for a long time.
Assume you have a script that takes a long time to complete. If you dedice 
to go for dinner, or leave school to go home, you would have to stop the script 
since it wouldn't be running anymore. 

.. _screen_sec:
------------
Screen
------------

The :code:`screen` program allows you to multiple virtual windows in **Unix**.

Some of the features of :code:`screen` are (from `this page <https://kb.iu.edu/d/acuy>`_ ):

* If your local computer crashes or you lose the connection, the processes or login sessions you establish through screen don't go away
    - You can resume your screen session with the command: :code:`screen -r`
    - In some cases you may have to manually *detach* your screen session before resuming it.
* The :code:`screen` program creates multiple processes instead of multiple Unix login sessions, which means that it is resource-efficient.
* You can cut and paste between different screens without using a mouse. Thus, you don't need to be on a computer with a windowing environment such as macOS, Windows, or the X Window System.
* It has a block copy feature which is similar to the kill rectangle feature of Emacs.
* You can copy and paste more than one page at a time, which you cannot do with some clients. You can scroll up more than one page, depending on how many scrolling lines you have set with the :code:`-h` option.
* Using the detach feature, you can save screen processes when logging out and resume where you left off, saving the trouble of restarting them.


+---------------------+---------------------------------------------------------------+
|Command              | Purpose                                                       |
+=====================+===============================================================+
|:code:`Ctrl-a c`     | Create new window (shell)                                     |
+---------------------+---------------------------------------------------------------+
|:code:`Ctrl-a k`     | Kill the current window                                       |
+---------------------+---------------------------------------------------------------+
|:code:`Ctrl-a w`     | List all windows (the current window is marked with "`*`")    |
+---------------------+---------------------------------------------------------------+
|:code:`Ctrl-a 0-9`   | Go to a window numbered 0-9                                   |
+---------------------+---------------------------------------------------------------+
|:code:`Ctrl-a n`     | Go to the next window                                         |
+---------------------+---------------------------------------------------------------+
|:code:`Ctrl-a Ctrl-a`| Toggle between the current and previous window                |
+---------------------+---------------------------------------------------------------+
|:code:`Ctrl-a [`     | Start copy mode                                               |
+---------------------+---------------------------------------------------------------+
|:code:`Ctrl-a ]`     | Paste copied text                                             |
+---------------------+---------------------------------------------------------------+
|:code:`Ctrl-a ?`     | Help (display a list of commands)                             |
+---------------------+---------------------------------------------------------------+
|:code:`Ctrl-a Ctrl-`\`| Quit screen                                                   |
+---------------------+---------------------------------------------------------------+
|:code:`Ctrl-a D`     | Power detach and logout                                       |
+---------------------+---------------------------------------------------------------+
|:code:`Ctrl-a d`     | Detach but keep shell window open                             |
+---------------------+---------------------------------------------------------------+

For some useful tutorials, see:

* `In Unix, what is screen, and how do I use it? <https://kb.iu.edu/d/acuy>`_ 
* `Learn to use screen, a terminal multiplexer <https://dev.to/thiht/learn-to-use-screen-a-terminal-multiplexer-gl>`_ 

.. _tmux_sec:
--------
Tmux
--------
  
For further reading and tutorials, see these:

* `A Gentle introduction to tmux <https://hackernoon.com/a-gentle-introduction-to-tmux-8d784c404340>`_ 








