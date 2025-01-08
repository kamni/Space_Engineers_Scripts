.. _commands:

Commands
========

.. note::

   Commands are not case-sensitive, unless specified otherwise.

.. _hotbar-commands:

Hotbar Commands
---------------

The following commands can be mapped to the hotbar of a command block:

.. _button-command:

BUTTON
  *Usage:*

  .. code::

     button_<#> <menu #>

  *Example:* Activate button 3 on menu 2

  .. code::

     button_3 2

  Activates button press for specified menu.

  The menu number can be found in the custom data of the desired menu LCD block.

  If the menu number is not supplied, the script will default to menu 1
  (this can be useful for ships with only one menu).

  The button number should correspond to the hotbar action it is mapped to.

.. _previous-page-command:

PREVIOUS_PAGE
  *Usage:*

  .. code::

    previous_page

  Changes specified Virtual Hotbar to the previous page.

  Rolls over to last page if current page is 1. 

.. _next-page-command:

NEXT_PAGE

  *Usage:*

  .. code::

     next_page

  Changes specified Virtual Hotbar to the next page.

  Rolls over to first page if currently on the last page. 

.. _utility-commands:

Utility Commands
----------------

The following commands can be run directly from the programmable block to
update the interface:

.. _refresh-command:

REFRESH
  *Usage:*

  .. code::

     refresh

  Rebuilds the program, updating LCD surfaces.

.. _set-grid-id-command:

SET_GRID_ID
  *Usage:*

  .. code::

     set_grid_id <optional gridID>

  Sets unique tag for the grid. The tag is case-sensitive.

  ``gridID`` is used to distinguish between other ships/stations when docking
  with merge blocks.
  If not specified, grabs the current in-game grid ID, which may be a GUID.

  Attribute is shared with other Laika Softworks scripts like
  `Pressure Chief <../pressure_chief/index.html>`_ and
  `USAP <../usap/index.html>`_.
  Command can be called from these other scripts as well.
