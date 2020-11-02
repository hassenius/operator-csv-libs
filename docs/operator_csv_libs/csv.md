Module operator_csv_libs.csv
============================

Classes
-------

`ClusterServiceVersion(csv, name=None, target_version=None, replaces=None, skiprange=None, logger=None)`
:   

    ### Class variables

    `LATEST_IMAGE_INDICATOR`
    :

    `RELATED_IMAGE_IDENTIFIER`
    :

    ### Methods

    `add_image_pullsecret(self, name)`
    :   Add image pull secret for all operator deployment deployments. Existing pull secrets will be kept
        
        Arguments:
            name {string|list} -- String or list of strings containing name of the pull secret to add

    `generate_spec_relatedImages(self)`
    :   Generates spec.relatedImages based on information found in operator deployment annotations marked with 'olm.relatedImage.*'

    `get_annotation_related_images(self)`
    :   Return a list of images found in 'olm.relatedImages.*' deployment annotations
        
        Returns:
            [List of Images] -- Returns a List of Images as defined in Images class

    `get_operator_deployments(self, api_version='apps/v1', kind='Deployment')`
    :   Return a list of kubernetes deployment objects constructed from the CSV deployments section
        
        Returns:
            [List fo Dict] -- List of kubernetes deployment objects

    `get_operator_images(self)`
    :   Return a list of images used for operator deployment
        
        Returns:
            [List of Images] -- Returns a List of Images as defined in Images class

    `get_owned_crds(self)`
    :   Returns a list of owned CustomResourceDefinitions
        
        Returns:
            [list [dict]]: List of owned custom resource definitions as dict object

    `get_replaces(self)`
    :   Return String
        
        Returns:
            String -- Returns the csv file name with previous version

    `get_updated_csv(self)`
    :   Returns the updated CSV object
        
        Returns:
            [dict] -- CSV with updated version and image information

    `set_deployments_annotations(self, key=None, value=None)`
    :   Set key with value passed in for each deployment in the CSV
        
        Arguments:
            key {string} -- key being search for in deployment annotations
            value {string} -- value that will be assigned to the key passed in

    `set_image_pullsecret(self, name)`
    :   Set the image pull secret for all operator deployment deployments. Overwrites any existing pull secret
        
        Arguments:
            name {string|list} -- String or list of strings containing name of the pull secret to add

    `set_replaces(self, replaces)`
    :   Set the release that this replaces
        
        Arguments:
            replaces {string} -- The versioned name of the csv that this csv replaces

    `set_version(self, version)`
    :   Set the target version for the CSV
        
        Arguments:
            version {string} -- Target version in semver format X.Y.Z with optional -nnnn for pre-release