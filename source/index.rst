.. Doing Getting Things Done under Linux slides file, created by
   hieroglyph-quickstart on Tue Apr 22 22:27:41 2014.


=======================================
Doing "Getting Things Done" under Linux
=======================================
:author: Craig Maloney <craig@decafbad.net>

:website: http://decafbad.net

Getting Things Done
===================
.. image:: /_static/Getting_Things_Done.jpg
    :scale: 50
    :align: right

Making It All Work
===================
.. image:: /_static/david-allen-gtd-making-it-all-work.jpg
    :scale: 50
    :align: right

What is GTD?
============

.. rst-class:: build
- GTD & Getting Things Done are registered trademarks of the David Allen Company.
- Commonly referred to as "Time Management".
- Really is a system for "Life Management" and "Focus Management".
- Completely technology independent (can use paper, computer, etc.)

Why do GTD at all?
==================

Getting Started
===============

Brief recap of GTD
==================

.. rst-class:: build

- Capture (Collect)
- Clarify (Process)
- Organize
- Reflect (Review)
- Engage (Do)

Capturing
=========

My Capture Tools
================
.. rst-class:: build

- Email inboxes (home and work)
- Evernote / Text Files
- Physical Inbox
- (Yes, physical is NOT Optional. :))
- Notepads / Moleskine / Fieldnotes (etc)

Why Physical?
=============
.. nextslide::
.. figure:: /_static/pre_inbox.jpg
   :class: fill

.. nextslide:: 
.. figure:: /_static/post_inbox.jpg
   :class: fill

Clarifying (Processing)
=======================

Key parts of a GTD system
=========================
.. rst-class:: build

- Context-based filtering
- Fast
- Flexible
- Fun to use

Why Todotxt?
============

.. rst-class:: build
- Context-based filtering
- Fast
- Flexible
- Fun to use
- Can be edited with vim (or any text editor)
- Easy to parse with UNIX tools

Basic Todotxt usage
===================
Adding a record::

   $ todo.sh add Draft up a presentation for GTD at +penguicon @computer
   187 Draft up a presentation for GTD at +penguicon @computer
   TODO: 187 added.

Basic Todotxt usage
===================
Listing based on context::

   $ todo.sh ls @computer
   187 Draft up a presentation for GTD at +penguicon @computer
   TODO: 1 of 187 tasks shown

Basic Todotxt usage
===================
Mark a Next Action as done:: 

   $ todo.sh do 187
   187 x 2014-04-30 Draft up a presentation for GTD at +penguicon @computer
   TODO: 187 marked as done.
   x 2014-04-30 Draft up a presentation for GTD at +penguicon @computer
   TODO: /home/craig/Dropbox/todo/todo.txt archived.

Basic Todotxt usage
===================

List contexts currently in use::

    $ todo.sh lsc
    @agenda
    @bills
    @calls
    @computer
    @errands
    @home
    @office
    @project
    @read
    @waiting

Basic Todotxt usage
===================

Todotxt can list on any keyword::

   craig@bluemidget:~$ t ls penguicon
   186 Bring in the luggage for Penguicon packing @home
   187 Draft up a presentation for GTD at +penguicon @computer
   162 Flesh out the slide outline for the GTD under Linux slides for Penguicon @computer
   067 Plan for Penguicon 2014 @project
   076 Present a GTD under Linux presentation at Penguicon @project
   --
   TODO: 5 of 187 tasks shown

Basic Todotxt usage
===================

Prioritize a next action::
    
    craig@bluemidget:~$ t pri 186 a
    186 (A) Bring in the luggage for Penguicon packing @home
    TODO: 186 prioritized (A).

    craig@bluemidget:~$ t ls penguicon
    186 (A) Bring in the luggage for Penguicon packing @home
    187 Draft up a presentation for GTD at +penguicon @computer
    162 Flesh out the slide outline for the GTD under Linux slides for Penguicon @computer
    067 Plan for Penguicon 2014 @project
    076 Present a GTD under Linux presentation at Penguicon @project
    --
    TODO: 5 of 187 tasks shown

Getting Things Done: Projects
=============================
.. rst-class:: build
- "Outcomes I want to have happen" list
- Clear statement of what you want to have true when complete:

  * "Garage" - What does "Garage" mean?
  * "Clean garage" - Getting warmer
  * "Clean and organize the garage so I can park the cars in there again" - Much better!

Projects under Todotxt
======================

.. rst-class:: build
- Limited to ``+project_name``
- Better served as keywords than a project list
- (I use a separate @projects context for my projects list)

Projects under Todotxt
======================


