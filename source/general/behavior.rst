General SSA and ASS Behavior
============================

.. toctree::
   :maxdepth: 3

SubStation Alpha is patterned on the Windows INI file format,
as such it retains certain hallmarks of the format such as the
usage of headings and the standard INI comment.

Default Style
-------------

The default ``Default`` style is as follows,
extra spaces are added to allow you to see what coresponds with
which style parameter.

Advanced SubStation Alpha Subtitles
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

    .. code-block:: INI

        [v4+ Styles]
        Format: Name,       Fontname,   Fontsize,   PrimaryColour,  SecondaryColour,    OutlineColour,  BackColour, Bold,   Italic, Underline,  StrikeOut,  ScaleX, ScaleY, Spacing,    Angle,  BorderStyle,    Outline,    Shadow, Alignment,  MarginL,    MarginR,    MarginV,    Encoding
        Style:  Default,    Arial,      18,         &H00FFFFFF,     &H00ffff00,         &H00000000,     &H00000080, 200,    0,      0,          0,          1,      1,      0,          0,      1,              2,          3,      2,          20,         20,         20,         1

SubStation Alpha Subtitles
~~~~~~~~~~~~~~~~~~~~~~~~~~

    .. code-block:: INI

        [v4 Styles]
        Format: Name,       Fontname,   Fontsize,   PrimaryColour,  SecondaryColour,    TertiaryColour, BackColour, Bold,   Italic, BorderStyle,    Outline,    Shadow, Alignment,  MarginL,    MarginR,    MarginV,    AlphaLevel, Encoding
        Style:  Default,    Arial,      18,         &H00FFFFFF,     &H00ffff00,         &H00000000,     &H00000080, 200,    0,      1,              2,          3,      2,          20,         20,         20,         0,          1


Unrecognized Headings and Entries
---------------------------------

Unrecognized headings and entries are to be ignored, it is up
to the implementation if a warning is produced in the logs.
