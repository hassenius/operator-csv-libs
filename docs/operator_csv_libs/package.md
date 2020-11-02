Module operator_csv_libs.package
================================

Classes
-------

`Channel(name, currentCSV)`
:   

    ### Methods

    `get_current_csv(self)`
    :

    `get_name(self)`
    :

    `set_current_csv(self, new_csv)`
    :

    `set_name(self, name)`
    :

`Package(package=None, operator=None, default_channel=None)`
:   

    ### Class variables

    `PACKAGE_FILE_FORMAT`
    :

    ### Methods

    `create_channel(self, name, current_csv, default=False)`
    :

    `get_channel(self, name)`
    :

    `get_channels(self)`
    :

    `get_formatted(self)`
    :

    `promote_channel(self, promote_from, promote_to)`
    :

    `set_default_channel(self, default_channel)`
    :

    `set_operator(self, operator)`
    :

    `update_channel(self, channel, new_csv)`
    :