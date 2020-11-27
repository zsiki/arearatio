# AreaRatio
QGIS plugin to calculate area ratio between a feature in a feature of a host 
polygon layer and other polygon layers.
This plug-in was written for local municipalities to calculate the percentage
of building footprints to the area of the parcel.

An icon with % will be added to the plug-ins toolbar if you turn it on.
A menu item *Area Ratio* will be added to the plug-in menu.

There are two class constants in PointTool class where you can set the name
of the layers to use with this plugin:

.. code:: python

    POLY_LAYER = "parcel"
    IN_POLY_LAYERS = ["living house", "garage"]

If there are more layers in the actual QGIS project with the given names, the 
first found will be used.
