#####
Setup
#####

.. _setup:

1. Load script onto a programmable block on the desired ship or station.
2. Rename block that contains screens with the tag [VHB]

   .. image:: images/setup-1-tag.jpg
      :width: 100%
      :alt: Example: adding [VHB] to the Flight Seat block.

   This can be a dedicated LCD block (like the Text Panel block).

   It can also a different terminal block with one or multiple display surfaces
   (like the Cockpit, Control Seat, Programmable Block, etc).

3. Run the program block with the argument REFRESH (not case sensitive).
4. Edit the Custom Data section of the LCD block to designate the desired
   buttons, icons, and actions.
5. In the hotbar for a desired control block map the button-press and page
   arguments as desired.

   .. image:: images/setup-2-button.jpg
      :width: 100%

   Control block can be same as LCD block (i.e. Cockpit)

   Control block can also be separate from LCD block.

   See the :ref:`Commands <commands>` section button-press and page arguments.
