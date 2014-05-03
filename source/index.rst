.. Doing Getting Things Done under Linux slides file, created by
   hieroglyph-quickstart on Tue Apr 22 22:27:41 2014.


=======================================
Doing "Getting Things Done" under Linux
=======================================
:author: Craig Maloney <craig@decafbad.net>

:website: http://decafbad.net

GTD Under Linux
===============
.. figure:: /_static/482225177_c083cff10f_o.jpg
   :class: fill

   http://www.flickr.com/photos/60849961@N00/482225177/ (BY-NC-ND)


Confession
==========
- Won't cover Tracks as much as I thought I might

  * http://getontracks.org

Sunday, 10am
============
.. figure::  /_static/5652854727_3bebef04d2_o.jpg
   :class: fill

   https://www.flickr.com/photos/gertcha/5652854727 (CC BY-ND)

Monday, 10am
============
.. figure:: /_static/4399026294_1f3906969d_o.jpg
   :class: fill

   https://www.flickr.com/photos/mandy_pantz/4399026294 (CC BY)

Recap of Getting Things Done
============================

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

Key elements of GTD
===================
.. rst-class:: build

- Capture everything that has your attention (inbox)
- Context-based: Filter based on what can you do at this moment
- Next Action list: List of physical actions to complete projects
- Project list: List of "successful outcomes"
- Calendar for "hard landscape" (appointments, day reminders).

Key elements of GTD
===================
.. rst-class:: build

- Waiting-for list (for items that you're waiting on other folks)
- Weekly review: system maintenance
- Horizons of focus (Roles, 1-5 year goals and plans, and life's-purpose)
- Someday / Maybe list (items you aren't committed to, but want to remember)

Brief recap of Five Phases of Work
==================================
.. rst-class:: build

- Capture (Collect)
- Clarify (Process)
- Organize
- Reflect (Review)
- Engage (Do)

Capturing
=========
.. rst-class:: build

- Any thought you have more than once should be captured
- Write it down!
- Meaning comes later. For now just dump.

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
.. rst-class:: build

- What is it? What's the next action?
- Two minute rule: If you can finish in less than two minutes, do it.
- One at a time: no batching
- Is it actionable? Reference? Trash?
- Nothing goes back into the in basket

Inbox Zero
==========

Organizing
==========
- No action?

  * Want to keep it? Reference.
  * Maybe want to do later? Someday / Maybe
  * Don't want / need it? **Throw it out**

Organizing
==========
- Actionable?

  * If more than one action, project list
  * Single action? Next Action list (with context)
  * Day-specific event? Calendar
  * Waiting for something to happen? Waiting for List.

Contexts
========
.. rst-class:: build

- Physical location where you can do something
- Example contexts

  * @computer
  * @home 
  * @calls
  * @agenda
  * @office
  * @errands

Reflect (Review)
================
.. rst-class:: build

- Review lists for next actions and things to check off
- Review project lists as needed to see what needs updating / completing
- Reference material for projects
- Mind sweep (anything that may need capturing)
- Occasionally: higher altitudes

Weekly Review: an aside
=======================

In other words
==============

DO YOUR WEEKLY REVIEW
=====================

DO YOUR WEEKLY REVIEW (Weekly)
==============================

Engage (Do)
===========
.. rst-class:: build

- Filter by:

  * Context (what can I do?)
  * Time available (what time do I have available?)
  * Energy (am I alert, or am I toast?)
  * Priority (Do you smell something burning?)

Engage (Do)
===========
.. rst-class:: build

- Three-fold nature of work:
  
  * Pre-defined work (Next action lists)
  * Defining your work (know ALL your work)
  * As it shows up (can lead to "busy-trap")


Key parts of a GTD system
=========================
.. rst-class:: build


- Context-based filtering
- Fast
- Flexible
- Fun to use

Todo.txt
========
.. image:: /_static/todotxt-apps_lrg.png 
    :align: right

Why Todotxt?
============

.. rst-class:: build

- Context-based filtering
- Fast
- Flexible
- Fun to use
- Can be edited with vim (or any text editor)
- Easy to parse with UNIX tools

What is Todo.txt?
=================
.. rst-class:: build

- A standardized text file-format for Next Actions
- A collection of applications for interfacing with a todo.txt file
- Cross-platform (CLI / Android / iOS)
- Developed by Gina Trapani and a dedicated community
- Free Software / Open Source
- Card-carrying Bad Ass Awesome
- (Available at http://todotxt.com)

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

Bash Aliases
============

    ``alias t='todo.sh'``

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

- Unfortunately, Todotxt doesn't have great project support baked in
- Limited to ``+project_name``
- Better served as keywords than a project list
- (I use a separate @projects context for my projects list)

Projects under Todotxt
======================
Project list best practice::

    t add Convert +penguicon slides to Hieroglyph @project
    t add Edit index.rst to copy the +penguicon slides over @computer
    t add Copy images for the +penguicon presentation to _static @computer

    craig@bluemidget:~$ t ls +penguicon
    188 Convert +penguicon slides to Hieroglyph @project
    190 Copy images for the +penguicon presentation to _static @computer
    187 Draft up a presentation for GTD at +penguicon @computer
    189 Edit index.rst to copy the +penguicon slides over @computer

Waiting for:
============
Making a "waiting for" next action::

    craig@gaplus:~$ t do 196
    196 x 2014-05-01 Put the final touches on the quarterly report for John @office
    TODO: 196 marked as done.
    x 2014-05-01 Put the final touches on the quarterly report for John @office
    TODO: /home/craig/Dropbox/todo/todo.txt archived.
    craig@gaplus:~$ t add John: OK with the quarterly report formatting / numbers @waiting
    195 John: OK with the quarterly report formatting / numbers @waiting
    TODO: 195 added.

List projects (tags)
====================
List the projects (tags)::

    craig@gaplus:~$ t lsprj
    +159
    +166
    +33
    +789
    +811
    +970
    +974
    +mug
    +openlab
    +penguicon
    +project_notes

Handy Addons
============

- schedule
- recur
- edit
- More at: https://github.com/ginatrapani/todo.txt-cli/wiki/Todo.sh-Add-on-Directory

Schedule
========
Add dates to next actions::

  craig@gaplus:~$ t ls +penguicon
  188 Convert +penguicon slides to Hieroglyph @project
  190 Copy images for the +penguicon presentation to _static @computer
  187 Draft up a presentation for GTD at +penguicon @computer
  189 Edit index.rst to copy the +penguicon slides over @computer
  --
  TODO: 4 of 194 tasks shown


Schedule
========
Add dates to next actions::

  craig@gaplus:~$ t schedule 190 thu
  190 Copy images for the +penguicon presentation to _static @computer due:2014-05-01

  craig@gaplus:~$ t v due +penguicon
  =====  Dates  =====

  ---  2014-05-01  ---
  190 Copy images for the +penguicon presentation to _static @computer

Recur
=====
- Recurring tasks (best with cron)

recur.txt::

  daily: Scoop Pixel's Poops @home
  friday: Ensure my timesheet is up to date and current @office

Running recur::

  craig@lister:~$ t recur
  194 Scoop Pixel's Poops @home
  TODO: 194 added.

Higher levels of focus
======================
Text files::

    craig@gaplus:~/gtd/weekly_review$ ls *rst
    20k-areas-of-focus.rst
    30k-1-2-year-goals.rst
    40k-vision.rst
    50k-purpose.rst
    setting_goals.rst
    weekly_review_checklist.rst
    work_goals_2013.rst

Someday / Maybe
===============
.. figure:: /_static/evernote.png
   :class: fill

What's the point of all this?
=============================
.. rst-class:: build

- Keep things off your mind
- Be present
- Know what you need to do
- Know what you're not doing

Questions?
==========
.. image:: /_static/todotxt-apps_lrg.png 
    :align: right

Links
=====
- http://gettingthingsdone.com
- http://todotxt.com
- http://getontracks.org
- http://evernote.com

Google+ Community
=================
.. image:: /_static/google_plus.png
    :align: right



Thank you!
==========

=======================================
Doing "Getting Things Done" under Linux
=======================================
:author: Craig Maloney <craig@decafbad.net>

:website: http://decafbad.net
