.. _configuration:


Configuration
=============

The X3D element supports a param tag which allows to set configuration for
the runtime.


Usage
-----
The param element behaves just like any other HTML element. It must be
nested below the scene element. For XHTML you can use the self-closing syntax,
for HTML a closing tag is mandatory::

    <x3d>
        <scene>
            <param name="showLog" value="true" ></param>
            ...
        </scene>
    </x3d>


Options
-------
The following table lists the parameters currently supported.

=================  =========================  ===========     =================================================
  Parameter          Values                     Default         Description
=================  =========================  ===========     =================================================
showLog	           true, false                false           Hide or display the logging console
showStat           true, false                false           Hide or display the statistics overlay
showProgress       true, false, bar           true            Hide or show the loading indicator. The default
                                                              indicator is a spinner. The value 'bar' will
                                                              use a progress bar.
PrimitiveQuality   High, Medium, Low, float   High/1.0        Render quality (tesselation level) for Box, Cone,
                                                              Cylinder, Sphere.
=================  =========================  ===========     =================================================
