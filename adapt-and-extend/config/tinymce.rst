TinyMCE configuration
=====================

.. include:: ../../_robot.rst

.. code:: robotframework
   :class: hidden

   *** Test Cases ***

   Show Mail setup screen
       Go to  ${PLONE_URL}/@@tinymce-controlpanel
       Capture and crop page screenshot
       ...  ${CURDIR}/../../_robot/tinymce-setup.png
       ...  css=#content

.. figure:: ../../_robot/tinymce-setup.png
   :align: center
   :alt: TinyMCE setup configuration

Here you can finetune the appearance and settings of TinyMCE, the default text editor.

On the "Plugins and Toolbar" screen, you can enable and disable buttons on TinyMCE's toolbar.

The "Spell Checker" section holds a special bonus: you can enable the "After The Deadline" spell checker, which will highlight not only spelling mistakes but also grammar errors and common writing style errors.

.. note::

   If you use the "After the Deadline" spellchecker in a security-conscious setting, or with many users, you are encouraged to set up your own instance of the server. The software is open-source, and not difficult to set up.

