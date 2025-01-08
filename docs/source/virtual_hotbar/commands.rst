.. _commands:

########
Commands
########

The following commands can be run directly from the programmable block,
but preferably should be mapped to the hotbar of a command block
(i.e. button panel/cockpit).

.. note::

   Commands are not case-sensitive;
   however arguments to the commands (e.g., grid ID) may be case-sensitive.

.. _refresh-command:

REFRESH
  *Usage:*

  .. code::

     refresh

  Rebuilds the program, updating LCD surfaces.

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

.. _set-grid-id-command:

SET_GRID_ID
  *Usage:*

  .. code::

     set_grid_id <optional tag>

  Sets unique tag for the grid.

  GridID is used to distinguish between other ships/stations when docking with
  merge blocks.

  Attribute is shared with other Laika Softworks scripts like Pressure Chief
  and USAP.

  Command can be called from these other scripts as well.

  Optional tag allows you to specify the GridID (text).
