.. _page-and-button-parameters:

Page and Button Parameters
==========================

.. note::

   Before setting the parameters for the pages/buttons, the
   `Menu Parameters <menu_parameters.html>`_ must be configured.

   After configuring the menu, be sure to run the
   `REFRESH <commands.html#refresh-command>`_ command.
   This will create headings and parameters that are configured in this section.

Parameters for the pages and buttons can be found in the Custom Data of the
menu block, below the Virtual Hotbar menu settings.


.. _page-parameters:

Page Parameters
---------------

.. TODO - screen shot of page parameters

In the menu, you can set the :ref:`number of pages <page-count-parameter>` that
the menu has.
For each page, you can optionally configure the display of the page.

**Title** - Title of the individual menu-page.
  This will display on the screen.

.. _button-parameters:

Button Parameters
-----------------

.. image:: images/page-and-button-parameters-1-main.jpg

**Block** - Name of individual block, block group, or program block activated by the button.
  * For Block Groups, insert G: before the name.
  * For Program Blocks, insert P: before the name.

**Block Label** - Name displayed above the button.
  By default, limited to 7 characters

**Action** - The action activated by the button press.
  For individual blocks and block groups, an (incomplete) list of actions can
  be found at the
  `Space Engineers Wiki <https://spaceengineers.wiki.gg/wiki/Space_Engineers_Wiki>`_.

.. TODO - find out which page should be used for the actions

**Action Label** - Label that appears on the button.
  * Can be single line of up to 7 characters or two lines of up to 7 characters each.
  * Include a space to get a double line text.
  * Can be substituted with an icon.

    .. seealso::

       Read more about `Icons <icons.html>`_

**Toggle Block** - Name of individual block that determines power status of the button.
  Optional. Can be left blank.

  By default, the power status (on/off) of the toggle block will determine
  whether the button is lit.

  Toggle block name can be followed by a semicolon and an argument to track
  other block statuses.

  .. seealso::

     For more information on toggle blocks, see the section on
     `Toggle Block Arguments <toggle_block_arguments.html>`_.

**Blink Length** - Approximate duration (in seconds) the button will blink after being pressed.
    Disabled when set to 0.

    When set in conjunction with Toggle Block parameter blink sequence ends in
    Toggle Block power status.
