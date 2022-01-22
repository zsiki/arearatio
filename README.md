# AreaRatio
QGIS plugin to calculate area ratio between a feature of a host polygon layer 
and the features within the host polygon in other layers.
This plug-in was written for local municipalities to calculate the percentage
of building footprints to the area of the parcel by clicking.

Two icons will be added to the plugins toolbar. A tool icon with % to select the
container polygon feature and an icon with %? to configure the tool.
Two menu items are also added to the plugin menu. *Area Ratio* to select the tool and
*Area Ratio Dialog* to change configuration.

The layers used in the area ratio calculation can be given in a configuration
file. The *default.cfg* from the plugin directory is loaded at start up.
The config file can contain one block (*layers*) and two variables
(*parcel*, *buildings*). Here is a sample configuration file:

```
    [layers]
    parcel = "parcel"
    buildings = ["living house", "garage"]
```

The user can set the container layer and the cointained layers in the
configuration dialog. In this dialig you can select from the loaded
polygon layers of the actual project.
If there are more layers in the actual QGIS project with the given names, the 
first found will be used.
