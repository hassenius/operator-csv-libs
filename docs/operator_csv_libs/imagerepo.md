Module operator_csv_libs.imagerepo
==================================

Classes
-------

`ArtifactoryRepo(image, artifactory_base=None, artifactory_user=None, artifactory_key=None, logger=None)`
:   

    ### Methods

    `get_image_digest(self)`
    :

    `get_manifest_list_digest(self)`
    :

    `get_raw_manifest_list(self)`
    :   Return the docker manifest list in json format
        Raises:
            ManifestListNotFound: [description]
        Returns:
            DICT: manifest.list.json content

`ImageRepo(image, logger=None)`
:   This is a class to provide a general interface to query container image registry servers.
    Hacked together in a hurry, will probably be refactored to be more pythonic - if there's a better way to do this

    ### Methods

    `get_image_digest(self)`
    :

    `get_manifest_list_digest(self)`
    :

    `get_raw_manifest_list(self)`
    :   Return the docker manifest list in json format
        Raises:
            ManifestListNotFound: [description]
        Returns:
            DICT: manifest.list.json content

`ManifestListNotFound(*args, **kwargs)`
:   Common base class for all non-exit exceptions.

    ### Ancestors (in MRO)

    * builtins.Exception
    * builtins.BaseException

`ManifestNotFound(*args, **kwargs)`
:   Common base class for all non-exit exceptions.

    ### Ancestors (in MRO)

    * builtins.Exception
    * builtins.BaseException

`MissingCredentials(*args, **kwargs)`
:   Common base class for all non-exit exceptions.

    ### Ancestors (in MRO)

    * builtins.Exception
    * builtins.BaseException

`QuayRepo(image)`
:   

    ### Class variables

    `QUAY_BASE_URL`
    :

    ### Methods

    `get_image_digest(self)`
    :

    `get_manifest_list_digest(self)`
    :

`RepoTypeNotImplemented(*args, **kwargs)`
:   Common base class for all non-exit exceptions.

    ### Ancestors (in MRO)

    * builtins.Exception
    * builtins.BaseException